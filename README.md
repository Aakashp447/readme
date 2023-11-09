# readme
![image](https://github.com/Aakashp447/readme/assets/92420490/74d8646f-bd6c-4edb-8d5f-95d45fb317a7)

- As shown in the image, we are going to create a new microservice named http-api-print-ready-srv. It will take input from FE and creates document into a jig collection like the collection named batches.
- After creating jig document event-print-ready will use that document and starts the actual process of creating jigs of ai files and png or PDF files in the proper needed format.
- After this, the printer user will get notified about the jig process. (It will be included later)
- In this, event-print-ready will work totally in the background due to it being a lengthy process.

*Doubts to discuss*
- For displaying cards into the printer MAT portal we will use API or direct FE call to db.
  If we are using API then this API will come under which service. (newly created http-api-print-ready-srv ?)
- All the APIs related to displaying jig status or information will come under newly created service named http-api-print-ready-srv, right?
- We need to decide on collection document architecture and provide a limit because if a very big document (having more than 1.04 MB size) comes then it can violate the document size limit for querying the database.
