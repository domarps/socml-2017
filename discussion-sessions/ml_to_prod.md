## ML in Production

### Agenda
- How to go about the transition of research to production?
- Do people prototype on a subset of data, then scale?
- What languages/toolsets are in use?
- What does the stack/pipeline look like?
- How is troubleshooting/maintenance/monitoring done?
- How is stability of updates ensured?
- How is integration with systems already running in production carried out?

### Tools/language in prod differ from research/dev
- get prod team to learn the new thing 
- onboarding new tools

### Post-sandbox mode, working with new tools 
- data engineers have to put in resources (cost)
- serialise the model (binary models -- java code that compiles to models -- decouples data structures used during (re-)training and prod)


### Dfferent dev-test-prod pipelines for online and offline ML systems
- Online (e.g. search product):
- elasticsearch over AWS to index embeddings
- FB open source tool for indexing -- nearest neighbour approach -- needs cluster of GPUs to take full advantage (https://github.com/facebookresearch/faiss)

### Scalability
- rewrite algorithms to work on distributed data
- Photon (https://engineering.linkedin.com/blog/2016/06/open-sourcing-photon-ml), scoring, training (reg, tree, GLM), more performant than SparkML
- on demand scoring
- caching
- getting data across is a bottleneck 
    -- on the fly composition (e.g. categorical to one hot) of data 


### Discussion about model's residence
- tf, protobuff, checkpoints, binaries 
- serialising simple models and moving to different framework (element analytics)
- data - scoring done offline, deliverable is hdfs, piped into API (github)
- `LASER` from linkedin
- consistent way of functioning across teams
- model as a service
- convincing others by demoing (DL in a box/AWS)
- decoupling dev env from prod env


### Separating research and product people
- company with money -- yes
- applied scientists --- must code
- small team, model does not matter, whole product has to be updated/shipped
- separation needs a strong technical solution to coherence across teams

### Teaching ML at University to make students ready for ML in production jobs OR do research with production in mind:
- go from code to fundamentals rather than the other way around (e.g. how fast.ai teaches)
- force ML ppl to make a product out of their projects/papers -- flask wrapper/API
