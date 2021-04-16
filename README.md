# practice

GETTING STARTED
- The template csv file should be saved in the same folder on the server as the images you are trying to upload
- Download the objectlist.csv file

- Import Image Template.csv
  - Fill out for files wanting to upload
  - First column = path of image, second column = first object number, third column = second object number (if only one object leave blank)

- TMS Image Import - Write CSV + Copy Images.ipynb
  - Use to copy images AND create csv to upload images
  - Set filepath = name of your template csv
  - Will ask for title the new csv file after running code
  - FindPythonFiles
        - Collects information from template and makes various lists, which will be used to make the new csv file
        - Makes dictionary, image path:object numbers
  - ObjectIdList
        - Takes object number and finds matching object id
  - CopyPhotos
        - Makes copy of image with name as object number (adds b if duplicate image)
  - RenameAndCopyPhotos
        - Makes copy of image with name as object number (adds b if duplicate image)
        - Creates ordered list to be used to make the new csv file
  - Renamer
        - Makes the new csv file to be used to upload the images to TMS
        - New csv file will be located in the same folder as the starting template csv

- TMS Image Import - Write CSV Only.ipynb
  - Use to create csv to upload images
  - Set filepath = name of your template csv
  - Will ask for title the new csv file after running code
  - FindPythonFiles
        - Collects information from template and makes various lists, which will be used to make the new csv file
        - Makes dictionary, image path:object numbers
  - ObjectIdList
        - Takes object number and finds matching object id
  - Renamer
        - Makes the new csv file to be used to upload the images to TMS
        - New csv file will be located in the same folder as the starting template csv

- objectlist.csv
  - List of every Museum specimen with its object number and official "other" number (object id)
  - Needed to make the second column of the spreadsheet and run ObjectIdList
