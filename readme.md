<h1 align='center'> Research Paper Analysis </h1>

<h2 align='left'>Idea </h2>
&nbsp;&nbsp;&nbsp; The General idea is that we are going to build a system capable of doing locating various segments of research papers like: 
    <ul>
        <li> Text </li>
        <li> Title </li>
        <li> Figures </li>
        <li> Tables </li>
        <li> References </li>
        <li> header </li>
    </ul>
We are also going to compare all the existing methods and check which ones perfom very well.<br><br> 

<h2 align='left'> 1. Paddle OCR </h2>
&nbsp;&nbsp;&nbsp; Initially we start with Paddle OCR and check how it performs for extraction of various components.<br><br>
Paddle OCR uses <b> Efficient and Accurate Scene Text detection (EAST)<b><br><br>
<h3> <b> Efficient and Accurate Scene Text detection (EAST): </b></h3><br>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Efficient and Accurate Scene Text Detection (EAST) is an algorithm for detecting text in natural scenes with high efficiency and accuracy. It was proposed by Xinyu Zhou, Cong Yao, He Wen, Yuzhi Wang, and Shuchang Zhou in their paper titled "EAST: An Efficient and Accurate Scene Text Detector". EAST uses a fully convolutional neural network (FCN) for text detection, which makes it faster than traditional methods that use region proposal algorithms.
<br>
EAST works by first converting an input image to a feature map using a VGG16 network, which is a convolutional neural network pre-trained on the ImageNet dataset. The feature map is then fed to the Region Proposal Network (RPN) to generate region proposals. In EAST, the RPN is replaced with a feature fusion module that generates feature maps at different scales. These feature maps are then used to generate region proposals using a sliding window approach.
<br>
The next step in EAST is to use the region proposals to generate score maps and geometry maps. The score map is used to indicate the probability of each pixel belonging to a text region, while the geometry map is used to predict the location and orientation of the bounding box for each text region.
<br>
Finally, the score and geometry maps are used to extract the text boxes using non-maximum suppression (NMS). NMS is used to eliminate redundant detections and to select the best text boxes based on their confidence scores.
<br>
EAST is known for its high accuracy and efficiency, and it has been widely used in various applications such as document recognition, license plate recognition, and scene text recognition.
<br>
In summary, EAST is an algorithm for detecting text in natural scenes that uses a fully convolutional neural network and a feature fusion module to generate region proposals. It then uses score and geometry maps to extract text boxes using non-maximum suppression.</p>
<br>
Repo to Padddle OCR: <a href='https://github.com/PaddlePaddle/PaddleOCR'> Paddle </a>
<br><br>
A Brief concept of Paddle can be gained from the image below: 

<img src='https://user-images.githubusercontent.com/25809855/186171245-40abc4d7-904f-4949-ade1-250f86ed3a90.png' algn='center'>
Here are some of the results we have obtained from Paddle COR:<br><br>
<h2> Results: </h2><br>

<table>
    <tr>
        <th> Original Images </th>
        <th> Paddle Ocr Image </th>
    </tr>
    <tr>
        <td><img src='Results/original_title.png' width="450" /></td>
        <td><img src='Results/paddle_title.png'  width="450" /> </td>
    </tr>
    <tr>
        <td><img src=Results/original_table_text_title.png width="450" /></td>
        <td><img src=Results/paddle_table_text_title.png  width="450" /> </td>
    </tr>
    <tr>
        <td><img src=Results/original_table_references.png width="450" /></td>
        <td><img src=Results/paddle_table_references.png  width="450" /> </td>
    </tr>
        
</table>


