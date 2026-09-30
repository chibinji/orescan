# OreScan

**An AI ore identification and grading tool to increase mining productivity in Zambia.**

> **Status:** Planning / early development. This repository documents the project plan and will be updated as the prototype is built.

## The problem

Many small-scale and artisanal miners, and some mid-sized operations, rely on manual visual inspection to tell valuable ore from waste rock. Misidentified material leads to wasted processing effort, lost revenue and lower output.

## The solution

OreScan lets a miner take a photo of a rock sample with a phone and get:

- the **ore type** (for example copper, cobalt, manganese or gemstones)
- an estimate of **relative quality**
- a recommendation on whether the material is worth processing

## How it will work

1. **Data:** collect and label photos of common Zambian ores, starting with public mineral image datasets and supplementing them with photos from partners such as the UNZA geology department and local mines.
2. **Model:** fine-tune a pretrained open-source computer vision model (for example ResNet, EfficientNet or a YOLO variant) using transfer learning.
3. **API:** serve the model through a REST API built with FastAPI.
4. **Front-end:** a lightweight, mobile-friendly web app where users upload or capture a photo and see the result.
5. **Open documentation:** setup guides, dataset notes and model cards so other student innovators can reuse and extend the work.

## Planned tech stack

| Layer | Tools |
|---|---|
| Model training | Python, PyTorch, torchvision, scikit-learn |
| Experiment tracking | Jupyter notebooks, Weights & Biases or TensorBoard |
| API | FastAPI, Uvicorn |
| Front-end | TypeScript, React or Next.js (mobile-first) |
| Deployment | Docker, UNZA AI UniPod GPU infrastructure |

## Roadmap

- [ ] Gather and label an initial ore image dataset
- [ ] Train a baseline classifier and record accuracy
- [ ] Improve the model with augmentation and fine-tuning
- [ ] Build the prediction API
- [ ] Build the mobile-friendly web app
- [ ] Test with real users (small-scale miners, geology students)
- [ ] Write documentation and a model card
- [ ] Explore extensions such as conveyor-belt sorting for larger mines

## Known limitations and risks

- Accuracy depends heavily on the quality and variety of the training images.
- Lighting, camera quality and rock surface conditions will affect results.
- OreScan is a decision-support tool. Its output should not replace laboratory assay testing.

## Sustainable Development Goals

- **SDG 8, Decent Work and Economic Growth:** raises output and income for miners.
- **SDG 9, Industry, Innovation and Infrastructure:** builds local AI capability for Zambia's key industry.
- **SDG 12, Responsible Consumption and Production:** reduces waste by processing the right material.
- **SDG 1, No Poverty:** helps small-scale miners earn fairer prices for their material.

## Author

**Samuel Chibinji Mwanza**
BSc Computer Science (4th year), University of Zambia
GitHub: [@chibinji](https://github.com/chibinji)

## Contributing

Contributions, ideas and dataset suggestions are welcome. Please open an issue to start a discussion.

## License

To be confirmed (MIT is planned).
