# desk-object-sorter-ai

## Project Description
A brief (1-2 sentence) description of your project. For example: "This project uses Google's Teachable Machine to classify common objects found on my desk."

## Classes Identified
List the objects your model was trained to identify:
* Keyboard
* Monitor
* Mouse
* Phone
* Decor
* Consumables
* Jakob

## Discussion & Reflection


1.  **Model Performance & Iteration:**

    My first trained model had only 3 classes and was pretty accurate. It could only correctly identify the objects it was trained on in very specific situations and often failed when the images looked slightly different.

    To improve the model, I added more images and classes and tried to include more variation for each class, such as different desks and angles. However, instead of improving performance, this actually made the model more confused. The accuracy decreased and the confidence scores became less reliable.

    These changes likely made the model worse because the added images introduced too much variation without enough clear distinction between classes. The model may have started focusing on background features like desks instead of the actual objects.

2.  **Challenges & Observations:**
   
    The easiest objects for the model to learn were those with very distinct visual features, such as unique shapes or colors. These stood out clearly and were easier for the model to recognize.

The most challenging objects were items that looked similar or appeared in similar environments, such as desk items like keyboards, phones, and other objects. Because they shared similar shapes and backgrounds, the model had difficulty telling them apart.

When I showed the model an object it was not trained on, it still tried to classify it as one of the known categories. For example, when I added a person, my coworker Jakob, the model identified him but also incorrectly labeled objects like a phone even when none was present. The confidence scores were sometimes high even when the prediction was wrong. This is significant because it shows that the model does not understand when it is incorrect and will always choose the closest match.

3.  **Bias in AI:**
   
    If I only trained the mug class using images of my specific mug, the model would not perform well when identifying other mugs. It would likely only recognize mugs that look very similar to mine. This demonstrates how bias can be introduced when training data is too limited or not diverse.

If all training images were taken in bright lighting, the model would likely perform poorly in dim lighting or with shadows. This shows that the model is not robust and can be biased toward the conditions it was trained in. Without variation, the model cannot generalize well to new situations.

4.  **Model Limitations & Usefulness:**
    
    Some key limitations of my model include its reliance on small and inconsistent datasets, its sensitivity to background and lighting, and its inability to recognize objects outside its training data. It also struggles with similar looking objects and can give high confidence predictions even when incorrect.

Downloading the trained model files is useful because it allows the model to be shared and reused. Files like model.json and weights.bin contain the learned patterns, which means the model can be used in other applications without retraining. This enables deployment in websites, apps, or further experimentation.

5.  **Real-World Applications & Ethics:**
   
    One real world application of image classification is in recycling systems, where objects can be sorted automatically based on their material. Another application is in retail, where items can be recognized for automatic checkout. A third example is assistive technology that helps visually impaired individuals identify objects around them.

One important ethical consideration is fairness. If the training data is not diverse, the model may perform poorly for certain groups or environments. This can lead to biased or unreliable outcomes, so it is important to carefully design and test AI systems before using them in real world situations.

## (Optional) Challenges Faced / Interesting Discoveries

One challenge I faced was that adding more images did not improve the model and actually made it worse. I also discovered that the model was heavily influenced by background features like desks. Another interesting observation was that the model could confidently make incorrect predictions, such as identifying a phone when none was present.

##  Screenshots 
V1
Here is my first attempt
<img width="1294" height="885" alt="ComputerVisionv1" src="https://github.com/user-attachments/assets/9499a69d-b775-44e4-8eb3-c169357ca9ab" />

V2
Second with more classes and a sort of tricky photo to analyze
<img width="1896" height="1025" alt="ComputerVisionv2" src="https://github.com/user-attachments/assets/5a137fda-7f0d-4f4e-be5b-34acde4167a5" />

V3
More varied training data, easier picture to analyze. 
<img width="868" height="880" alt="Screenshot 2026-04-27 111044" src="https://github.com/user-attachments/assets/6d64b9a4-1bb0-4d91-b062-a49e7b3e07ca" />
