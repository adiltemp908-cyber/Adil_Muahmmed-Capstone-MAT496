# Title: LLM Amazon Affiliate Business

---

## Overview

The vision is to have a llm equiped with amazon dataset who will shortlist the items from database based on the users requirements and provide further details and reviews from websearch. The link will be replaced with our affliate link. This can be advertised on a platfrom as a new way to search for products as amazon just shows promoted advertised products or their own products first. This is a way to get users to use this service and generate generate business

---

## Reason for Picking Up This Project

The first idea was selective news where the user asks for specific categories which llm provides but it was too basic. The new plan will be harder to do but more interesting. The plan is to download a huge dataset fro kaggle then upload it to langsmith. Use RAG and Semantic search for better implementaion of llm and course purposes. Do parallel web search for final shortlisted items from users requirements but when pren presenting the links replace it with our affliate link by adding the affliate tag. This part wont be fully implemented tho as you need to have a website to your name and get verified by amazon. This function will remain but just as proof of concept. And finally I will build the nodes and graphs showing the workings and parallel components. So after everything all the concepts that we needed to learn throughout the course will be used in this project.

---

## Plan

I plan to execute these steps to complete my project:

- [DONE] Step 1 Downloading the amazon sub Dataset from kaggle and then formating it and upload to langsmith database. This process failed at beginning due to size constraints then I uploaded it in chunks. Fun fact- The uploading process alone took 34 minutes.
  <img width="1561" height="1046" alt="image" src="https://github.com/user-attachments/assets/86a3fe8c-a4b6-4532-a7ff-c7315ae889ba" /> <br>

 
- [Done] Step 2 Vectoring or making the the database into the from for semantic search. This step came with lots of difficulties. First of all langsmith has paywall for database indexing so the embedding has to be done locally. OpenAI embedding was initiated but at just 1% progress it ate $1 so it was stopped. Now the only option was to use less powerfull, less accurate and more time consuming free embedding options. One attempt reached 90% progress and then failed after 72 min.
  <img width="1549" height="1006" alt="Screenshot 2025-11-27 185229" src="https://github.com/user-attachments/assets/b03a3316-c9c5-4b69-b9df-29ca3126ec4c" /> <br> 
  The next attempt used different embedding but also failed after 5 hours
  <img width="1588" height="615" alt="Screenshot 2025-11-28 075946" src="https://github.com/user-attachments/assets/0536196e-eb70-483b-a8e9-07af2c968590" />  <br>
 Finally successfull
  <img width="1566" height="805" alt="Screenshot 2025-11-28 125819" src="https://github.com/user-attachments/assets/50d4055f-64c6-466f-bfd2-1c47bd7474ae" /> <br> 
- [TODO] Step 3 From here I started building the actual notebook. Did the elementary steps here of importing, setting up different things and defined some of the functions
- [TODO] Step 

---

## Conclusion

I had planned to achieve {this this}. I think I have/have-not achieved the conclusion satisfactorily.  
The reason for your satisfaction/unsatisfaction.

