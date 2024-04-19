# BEQN_problem

## I am using the Storage Access Framework (SAF) to access directories and obtain the content URI of the directory to access the files.

## Here is the code 

 Intent i = new Intent(Intent.ACTION_OPEN_DOCUMENT_TREE); \
 intent.setType("*/*") \
 startActivityForResult(i, 9999);

## The error is 

android.content.ActivityNotFoundException: No Activity found to handle Intent { act=android.intent.action.OPEN_DOCUMENT_TREE flg=0x1 }



