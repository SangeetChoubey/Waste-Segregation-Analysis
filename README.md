# Waste Material Segregation for Improving Waste Management

## Objective
This project implements a **waste material segregation system** using **Convolutional Neural Networks (CNNs)** to classify waste into seven categories: Food Waste, Metal, Paper, Plastic, Other, Cardboard, and Glass. The system aims to **enhance recycling efficiency, reduce landfill waste, and promote sustainable waste management**.

## Dataset
The dataset contains images organized into folders by class:  

- Food Waste  
- Metal  
- Paper  
- Plastic  
- Other  
- Cardboard  
- Glass  

Each folder contains images of objects belonging to that category. For example, the `Food_Waste` folder may include coffee grounds, teabags, and fruit peels, without further subcategorization.

## Models
Two models were implemented and evaluated:  

1. **Custom CNN**  
   - 3 convolutional layers + dense layers  
   - Dropout for regularization  
   - Trained from scratch  

2. **ResNet50 (Transfer Learning)**  
   - Pretrained ImageNet backbone  
   - Dense head with dropout  
   - Fine-tuned for waste classification  

## Results
**Test Performance:**

**Custom CNN:**  
- Accuracy: 30%  
- Macro Precision: 19%  
- Macro Recall: 15%  
- Macro F1-score: 7%  

**ResNet50:**  
- Accuracy: 84%  
- Macro Precision: 83%  
- Macro Recall: 85%  
- Macro F1-score: 84%  

**Insight:** Transfer learning significantly outperforms training from scratch. ResNet50 provides robust feature extraction and balanced predictions.
