# Voice-Enabled-Photo-Search-Album-Frontend
## A simple frontend application that allows users to:
1. Make search requests to the GET /search endpoint
2. Display the results (photos) resulting from the query
   * Upload new photos using the PUT /photos
   * In the upload form, allow the user to specify one or more
   custom labels, that will be appended to the list of labels
   detected automatically by Rekognition
   * These custom labels should be converted to a
   comma-separated list and uploaded as part of the S3
   object’s metadata using a x-amz-meta-customLabels9
   metadata HTTP header.

3. Create a S3 bucket for your frontend (B1).
4. Set up the bucket for static website hosting (same as HW1).
5. Upload the frontend files to the bucket (B2).
6. Integrate the API Gateway-generated SDK (SDK1) into the frontend, to
   connect your API.


## Implemented Voice accessibility in the frontend
1. Give the frontend user the choice to use voice rather than text to perform
the search.
2. Use Amazon Transcribe on the frontend to transcribe speech to text10
(STT) in real time , then use the transcribed text to perform the search,11
using the same API like in the previous steps.


