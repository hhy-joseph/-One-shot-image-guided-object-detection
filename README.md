# -One-shot-image-guided-object-detection
Using OWL-ViT to perform One-shot / image-guided object detection


The OWL-ViT is an open-vocabulary object detector that uses CLIP with a ViT-like Transformer as its backbone to perform zero-shot text-conditioned object detection. Unlike traditional object detection models, OWL-ViT is not trained on labeled object datasets and leverages multi-modal representations. The model removes the final token pooling layer of the vision model and attaches a lightweight classification and box head to each transformer output token for object detection. Open-vocabulary classification is enabled by replacing the fixed classification layer weights with the class-name embeddings obtained from the text model. One or multiple text queries per image can be used for detection, and the model is trained using a bipartite matching loss. In this document, we demonstrate one-shot/image-guided object detection using the examples of a cat and Agumon.
