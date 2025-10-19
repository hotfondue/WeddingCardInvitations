# WeddingCardInvitations
## A simple script for populating and sharing wedding invitations over whatsapp based on an excel tracker.

_This script is designed to suit my personal prefernces and will need to be edited to suit yours._

This repo is designed keeping Indian/large weddings in mind, wherein you have multiple functions and multiple guests. But not every guest is invited to every function. This is a means to auto-populate sshare your invitations. 

These can be printed from the or sent over whatsapp as an e-invitation based on the tracker.

You will need a pdf card template and an excel tracker in the same format as given.

You can edit the python script according to the columns in your tracker, your conditions and the coords where you want to print your text within your template.  

STEPS:

1. Unzip WeddingCardInvitation.zip. 
2. Replace 'shaadi_invitation_template.pdf' with your card template, and the coords in the script accordingly.
3. Replace 'shaadi_guest_list.xlsx' with your tracker. This tracker must be pre filled with your guest details.
4. Install google chrome and replace 'chromedriver.exe' with the chromdriver matching your chrome version if needed.
5. Download python and install pip or conda. Im using conda.
6. Open anaconda console. Run the following commands:

```bash
conda create --name wedding_invitations
conda activate wedding_invitations
cd <path_to_WeddingCardInvitation_folder>
conda install pillow pandas reportlab
conda install -c conda-forge selenium
pip install PyPDF2
pip install openpyxl
```
8. Now run the following to execute your script:
```bash
python generate_cards.py
```
