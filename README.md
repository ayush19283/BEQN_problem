# BENQ_problem

## Our Use case : 
++++++++++++++

We store video and pdf files in a pen drive. We insert the pen drive to a smart panel with android 11. In our app 
We set the input folder and get the content URI. 

## Problem:
+++++++
On recent Android 11 on a particular panel (BenQ), when we are trying to access the pen drive, it does not work.\
   
  Note that it works on Android 11 on a phone . 

  
## Diagnostic Analysis:
====================

   To debug the issue, we have created a standalone test case. I am sharing the git Repo and apk.

## I am using the Storage Access Framework (SAF) to access directories and obtain the content URI of the directory to access the files.

## Here is the code 

 Intent i = new Intent(Intent.ACTION_OPEN_DOCUMENT_TREE); \
 intent.setType("*/*") \
 startActivityForResult(i, 9999);

## The error is 

android.content.ActivityNotFoundException: No Activity found to handle Intent { act=android.intent.action.OPEN_DOCUMENT_TREE flg=0x1 }



