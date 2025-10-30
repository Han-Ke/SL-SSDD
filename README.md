# SL-SSDD
SL-SSDD: Sea-Land Segmentation Dataset for SSDD
SL-SSDD is the first synergistic sea-land segmentation dataset tailored for deep learning-based SAR ship detection, built upon the well-established SAR Ship Detection Dataset (SSDD). It addresses the critical gap of lacking sea-land prior information in existing SAR ship detection datasets, enabling models to fully distinguish between sea and land regions for more accurate detection.
🔍 Core Features
Pixel-Level Sea-Land Annotations: Each image is paired with a PNG-format segmentation mask (same filename as SSDD images) where pixel 0 denotes land and 255 denotes sea. Annotations are completed by SAR interpretation experts, ensuring precise coastal contours and offshore topography capture.
Seamless Compatibility: Directly complements SSDD (1160 SAR images, 2456 ship targets from TerraSAR-X, RadarSat-2, Sentinel-1) without additional data modification, supporting both 8:2 train-test split and original SSDD experimental settings.
Dual Application Paradigms:Priors-Available Scenario: Input both SAR images and sea-land masks to guide models (e.g., SLA-Net) in focusing on valuable sea/ship regions.
Priors-Unavailable Scenario: Use masks as auxiliary labels to train sea-land segmentation capabilities (supervised/unsupervised) for subsequent ship detection.
Open & Reproducible: Publicly accessible with standardized annotations, facilitating fair comparison and advancing research on synergy between sea-land segmentation and SAR ship detection.
🎯 Key Value
SL-SSDD effectively mitigates land-based false alarms (e.g., containers, coastal structures) and inshore ship missed detections by providing critical sea-land semantic priors. It empowers models to enhance feature extraction in sea regions, suppress land interference, and improve performance on small ships, nearshore complex scenes, and multiscale targets—addressing long-standing challenges in SAR ship detection.
📥 Download & Citation
Dataset Link: https://github.com/Han-Ke/SL-SSDD
Citation: Ke, H.; Ke, X.; Zhang, Z.; Chen, X.; Xu, X.; Zhang, T. SLA-Net: A Novel Sea–Land Aware Network for Accurate SAR Ship Detection Guided by Hierarchical Attention Mechanism. Remote Sens. 2025, 17, 3576. https://doi.org/10.3390/rs17213576
We welcome researchers to use SL-SSDD for SAR ship detection, sea-land segmentation, and related cross-task studies. Feel free to raise issues or submit pull requests for improvements!
