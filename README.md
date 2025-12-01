# Title: LLM Amazon Affiliate Business

---

## Overview

The vision is to have a llm equiped with amazon dataset who will shortlist the items from database based on the users requirements and provide further details and reviews from websearch. The link will be replaced with our affliate link. This can be advertised on a platfrom as a new way to search for products as amazon just shows promoted advertised products or their own products first. This is a way to get users to use this service and generate  business.<br>
Video link - https://drive.google.com/file/d/1JBkrJHbkzKlbokW94xzjM88p8KelGUHE/view?usp=sharing

---

## Reason for Picking Up This Project

The first idea was selective news where the user asks for specific categories which llm provides but it was too basic. The new plan will be harder to do but more interesting. The plan is to download a huge dataset fro kaggle then upload it to langsmith. Use RAG and Semantic search for better implementaion of llm and course purposes. Do parallel web search for final shortlisted items from users requirements but when pren presenting the links replace it with our affliate link by adding the affliate tag. This part wont be fully implemented tho as you need to have a website to your name and get verified by amazon. This function will remain but just as proof of concept. And finally I will build the nodes and graphs showing the workings and parallel components. So after everything all the concepts that we needed to learn throughout the course will be used in this project.

---

## Plan

I plan to execute these steps to complete my project:

- [DONE] Step 1 Downloading the amazon sub Dataset from kaggle and then formating it and upload to langsmith database. This process failed at beginning due to size constraints then I uploaded it in chunks. Fun fact- The uploading process alone took 34 minutes.
  <img width="1561" height="1046" alt="image" src="https://github.com/user-attachments/assets/86a3fe8c-a4b6-4532-a7ff-c7315ae889ba" /> <br><br>
- [Done] Step 2 Vectoring or making the the database into the from for semantic search. This step came with lots of difficulties. First of all langsmith has paywall for database indexing so the embedding has to be done locally. OpenAI embedding was initiated but at just 1% progress it ate $1 so it was stopped. Now the only option was to use less powerfull, less accurate and more time consuming free embedding options. One attempt reached 90% progress and then failed after 72 min.
  <img width="1549" height="1006" alt="Screenshot 2025-11-27 185229" src="https://github.com/user-attachments/assets/b03a3316-c9c5-4b69-b9df-29ca3126ec4c" /> <br> <br>
  The next attempt used different embedding but also failed after 6 hours
  <img width="1588" height="615" alt="Screenshot 2025-11-28 075946" src="https://github.com/user-attachments/assets/0536196e-eb70-483b-a8e9-07af2c968590" />  <br><br>
 Finally successfull after another 5 hour attempt
  <img width="1566" height="805" alt="Screenshot 2025-11-28 125819" src="https://github.com/user-attachments/assets/50d4055f-64c6-466f-bfd2-1c47bd7474ae" /> <br> <br>
- [DONE] Step 3 From here I started building the actual notebook. Did the elementary steps here of importing, setting up different things and defined some of the functions. <br><br>
- [DONE] Step 4 I completed defining all functions and created langgraph.
  <img width="1301" height="952" alt="Screenshot 2025-11-28 154615" src="https://github.com/user-attachments/assets/586b472e-ce37-4f0b-a132-b7c28432fcf9" /> <br><br>
- [DONE] Step 5 I fixed a lot of errors that became visible when finally running the code. So this was debugging phase. <br><br>
- [DONE] Step 6 Now I am going to upload the file. I will also run it a few times and get examples to show here.


---

## Example runs (Outputs)

First Example
<img width="1543" height="996" alt="Screenshot 2025-11-29 003315" src="https://github.com/user-attachments/assets/baa3ba6b-c8d4-4b74-8db7-180407bfbee2" />
<img width="1531" height="1026" alt="Screenshot 2025-11-29 003344" src="https://github.com/user-attachments/assets/5a1b7f1b-cfcb-4141-9495-a644754209e5" />
<img width="1546" height="834" alt="Screenshot 2025-11-29 003408" src="https://github.com/user-attachments/assets/c3089e22-192b-42d3-85e6-63afe66c44a2" />
<img width="1545" height="744" alt="Screenshot 2025-11-29 003054" src="https://github.com/user-attachments/assets/7fd76fb3-5e22-4250-92b4-26233aa2024e" />
<br><br>
Second example
<img width="1513" height="1017" alt="Screenshot 2025-11-29 000944" src="https://github.com/user-attachments/assets/c820ab85-77d9-4c12-882e-68cfe7612335" />
<img width="1512" height="999" alt="Screenshot 2025-11-29 001016" src="https://github.com/user-attachments/assets/0efe6e6a-f7e1-4f88-b641-7cd0f7b0cd17" />
<img width="1517" height="962" alt="Screenshot 2025-11-29 001059" src="https://github.com/user-attachments/assets/6c6c3d71-3cae-4648-8803-48df25f13a2e" />
<img width="1570" height="815" alt="Screenshot 2025-11-29 000733" src="https://github.com/user-attachments/assets/735a00d9-d752-4ec5-b8d2-4a6e81ec27af" /> <br><br>
Third example
<img width="1522" height="971" alt="Screenshot 2025-11-28 231648" src="https://github.com/user-attachments/assets/48216a21-bde7-4f91-8bda-cc1ce2436248" />
<img width="1496" height="1017" alt="Screenshot 2025-11-28 231725" src="https://github.com/user-attachments/assets/0a241f54-f75c-43a8-9d0b-e4d731407c83" />
<img width="1456" height="917" alt="Screenshot 2025-11-28 224025" src="https://github.com/user-attachments/assets/0f6523df-1047-42d8-91f1-6e43fc58978e" /> <br>




---

## Conclusion

The initial plan and all of its components have been achieved although not perfectly. Problems with the final state:
- The dataset used is of 2023 as other upto datesets were hard to find or behind paywall. Due to this as visible in the example run a lot of the products are currently unavailable.
- Vectoring process of dataset saved in langsmith is behind their subscription. Furthermore local vectoring of openai was extremely token intensive making that also behind paywall. So had to resort to local free vectoring which    in turn is highly cpu intensisve. This led to many crashes of laptop during random times and worse search results.
- Amazon affliate verification has not been obtained yet so in the function it is currently returning original link itself. If affliate tag is obtained changing a flag in the function will make it return affliate link.

So in conclusion some features that can make this project come to full vision are behind paywall. But still all components are functioning as required and what I set out to achieve intially was achieved.The project also implemented all the course elements we were suppossed to and more like parallelization and other stuff. I initially did not expect it to function at this level so I am pleasently surprised.
