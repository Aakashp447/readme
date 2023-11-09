# readme
![image](https://github.com/Aakashp447/readme/assets/92420490/80e7576e-bcdc-41cd-aab1-78088f5ddb10)

- As shown in image, we are going to create a new microservice named http-api-print-ready-srv. It will take input from FE and creates document into jig collection like batches collection.
- After creating jig document event-print-ready will use that document and starts the actual process of creating jigs of ai files and png or pdf files.
- After this, printer user will get to notify about jig process. (It will include later)
- In this, event-print-ready will work totally in background due to it is a lengthy process.

*Doubt*
- For displaying cards into printer MAT portal we will use API or direct FE call to db.
  If we are using API then this API will come under which service. (newly created http-api-print-ready-srv ?)
- All the APIs related to display jig status or information will come under newly created service named http-api-print-ready-srv, right ?
- We need to decide collection document architecture and need to provide limit because if very big document (having more than 1.04 mb size) came than it can violate document size limit for querying database.
