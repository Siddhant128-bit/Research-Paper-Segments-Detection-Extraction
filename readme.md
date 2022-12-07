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


