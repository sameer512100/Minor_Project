# CNN + CapsGNN Architecture (Compact)

```mermaid
flowchart TD
    A[Input Image<br/>224 x 224 x 3]
    B[Preprocessing<br/>Resize + Normalize + Augment]
    C[CNN Backbone<br/>ResNet18]
    D[Primary Capsules<br/>Feature to Capsule Tokens]
    E[Capsule Graph + GNN<br/>k-NN + 2 GraphConv]
    F[Readout + Classifier<br/>Mean Pool + FC]
    G[Output<br/>8 GI Classes]

    A --> B --> C --> D --> E --> F --> G
```
