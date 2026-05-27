# Frameworks — Jure Leskovec

## GNN Drug Discovery Pipeline
1. **Knowledge graph construction**: Genes, proteins, diseases, drugs, phenotypes
2. **GNN training**: Learn node embeddings from graph structure
3. **Link prediction**: Predict drug-target, drug-disease, drug-drug interactions
4. **Experimental validation**: Test top predictions in vitro/in vivo
5. **Iteration**: Use experimental results to improve model

## GraphSAGE Workflow
1. **Sample neighbors**: For each node, sample a fixed-size neighborhood
2. **Aggregate**: Aggregate neighbor features using mean/LSTM/pooling
3. **Update**: Update node representation with aggregated features
4. **Repeat**: Apply multiple layers for multi-hop aggregation
5. **Predict**: Use final node representations for downstream tasks
