# Comparing `tmp/SATO-0.1.5.tar.gz` & `tmp/SATO-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SATO-0.1.5.tar", last modified: Fri Mar 15 06:15:21 2024, max compression
+gzip compressed data, was "SATO-0.1.6.tar", last modified: Sun Apr 28 13:55:14 2024, max compression
```

## Comparing `SATO-0.1.5.tar` & `SATO-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-03-15 06:15:21.179386 SATO-0.1.5/
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     1069 2024-03-13 17:18:07.000000 SATO-0.1.5/LICENSE
--rw-r--r--   0 clabe     (1000) clabe     (1000)     6809 2024-03-15 06:15:21.179386 SATO-0.1.5/PKG-INFO
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     5669 2024-03-15 06:12:30.000000 SATO-0.1.5/README.md
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-03-15 06:15:21.179386 SATO-0.1.5/SATO/
--rw-rw-r--   0 clabe     (1000) clabe     (1000)    35061 2024-03-14 06:43:23.000000 SATO-0.1.5/SATO/SATO.py
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       43 2024-03-14 06:50:55.000000 SATO-0.1.5/SATO/__init__.py
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     2352 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/about_intro.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     3197 2024-03-15 06:13:15.000000 SATO-0.1.5/SATO/help.txt
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-03-15 06:15:21.179386 SATO-0.1.5/SATO/icons/
--rw-rw-r--   0 clabe     (1000) clabe     (1000)    22650 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/icons/download.png
--rw-rw-r--   0 clabe     (1000) clabe     (1000)   216311 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/icons/fasta.png
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     1354 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/icons/file.png
--rw-rw-r--   0 clabe     (1000) clabe     (1000)    53857 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/icons/logo-no-background.png
--rw-rw-r--   0 clabe     (1000) clabe     (1000)    67297 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/icons/sato.png
--rw-rw-r--   0 clabe     (1000) clabe     (1000)      512 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/stylesheet.css
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     3298 2024-03-13 17:18:07.000000 SATO-0.1.5/SATO/validation.py
-drwxrwxr-x   0 clabe     (1000) clabe     (1000)        0 2024-03-15 06:15:21.179386 SATO-0.1.5/SATO.egg-info/
--rw-r--r--   0 clabe     (1000) clabe     (1000)     6809 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/PKG-INFO
--rw-rw-r--   0 clabe     (1000) clabe     (1000)      426 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/SOURCES.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)        1 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/dependency_links.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       40 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/entry_points.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       16 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/requires.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)        5 2024-03-15 06:15:21.000000 SATO-0.1.5/SATO.egg-info/top_level.txt
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       70 2024-03-13 17:18:07.000000 SATO-0.1.5/run.py
--rw-rw-r--   0 clabe     (1000) clabe     (1000)       38 2024-03-15 06:15:21.179386 SATO-0.1.5/setup.cfg
--rw-rw-r--   0 clabe     (1000) clabe     (1000)     1729 2024-03-14 06:49:00.000000 SATO-0.1.5/setup.py
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1069 2024-03-13 17:18:07.000000 SATO-0.1.6/LICENSE
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-28 13:55:14.025518 SATO-0.1.6/PKG-INFO
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     5669 2024-03-15 06:12:30.000000 SATO-0.1.6/README.md
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO/
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)    33330 2024-04-28 13:48:12.000000 SATO-0.1.6/SATO/SATO.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       43 2024-04-28 13:20:29.000000 SATO-0.1.6/SATO/__init__.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     2352 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/about_intro.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3197 2024-03-15 06:13:15.000000 SATO-0.1.6/SATO/help.txt
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO/icons/
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    22650 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/download.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)   216311 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/fasta.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1354 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/file.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    53857 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/logo-no-background.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)    67297 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/icons/sato.png
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      512 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/stylesheet.css
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     3298 2024-03-13 17:18:07.000000 SATO-0.1.6/SATO/validation.py
+drwxrwxr-x   0 cwekesa   (1000) cwekesa   (1000)        0 2024-04-28 13:55:14.025518 SATO-0.1.6/SATO.egg-info/
+-rw-r--r--   0 cwekesa   (1000) cwekesa   (1000)     6809 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/PKG-INFO
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)      436 2024-04-28 13:55:14.000000 SATO-0.1.6/SATO.egg-info/SOURCES.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        1 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/dependency_links.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       40 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/entry_points.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       16 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/requires.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)        5 2024-04-28 13:55:13.000000 SATO-0.1.6/SATO.egg-info/top_level.txt
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       70 2024-03-13 17:18:07.000000 SATO-0.1.6/run.py
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)       38 2024-04-28 13:55:14.029518 SATO-0.1.6/setup.cfg
+-rw-rw-r--   0 cwekesa   (1000) cwekesa   (1000)     1729 2024-04-28 13:20:15.000000 SATO-0.1.6/setup.py
```

### Comparing `SATO-0.1.5/LICENSE` & `SATO-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/PKG-INFO` & `SATO-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATO
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods
 Home-page: https://github.com/clabe-wekesa/SATO
 Author: Clabe Wekesa
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Keywords: consensus,alignment,phylogenetics,bioinformatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SATO-0.1.5/README.md` & `SATO-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/SATO.py` & `SATO-0.1.6/SATO/SATO.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PyQt6.QtCore import Qt, QFile, QTextStream, QIODevice
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio import AlignIO
 from io import StringIO
 import subprocess
 import shutil
-from .validation import (
+from validation import (
     is_protein_alignment, text_formatting,is_valid_fasta,
     is_fasta_aligned, is_valid_fasta
 )
 
 # Define a custom exception for your application
 class CustomError(Exception):
     def __init__(self, message):
@@ -545,271 +545,236 @@
         input_file = self.upload_path
         if not input_file:
             # Display an error message using the custom dialog
             error_message = "Please select a FASTA file to process."
             error_dialog = ErrorDialog(error_message)
             error_dialog.exec()
             return
-
-        # Generate the output file name based on the input file name
-        base_name = os.path.splitext(os.path.basename(input_file))[0]
-        output_file = f"{base_name}_cleaned.fasta"
-
+    
         try:
             with open(input_file, 'r') as f:
                 file_content = f.read()
-
+    
             # Check if the file content follows FASTA format
             if not is_valid_fasta(file_content):
                 error_message = "Selected file is not a valid FASTA file."
                 error_dialog = ErrorDialog(error_message)
                 error_dialog.exec()
                 return
-
+    
             # Generate the output file name based on the input file name
             base_name = os.path.splitext(os.path.basename(input_file))[0]
             output_file = f"{base_name}_cleaned.fasta"
-
+    
             current_sequence = ""
             sequences = []
-
+    
+            current_header = ""  # Initialize current_header
             for line in file_content.split('\n'):
                 line = line.strip()
                 if line.startswith(">"):
                     if current_sequence:
                         cleaned_sequence = self.remove_non_nucleotides(current_sequence)
                         sequences.append((current_header, cleaned_sequence))  # Store both header and sequence
                     current_sequence = ""
                     current_header = line
                 else:
                     current_sequence += line
-
+    
             if current_sequence:
                 cleaned_sequence = self.remove_non_nucleotides(current_sequence)
                 sequences.append((current_header, cleaned_sequence))  # Store both header and sequence
-
+    
             with open(output_file, 'w') as f:
-                for i, (header, sequence) in enumerate(sequences):
+                for header, sequence in sequences:
                     f.write(header + "\n")  # Write the header to the output file
                     f.write(sequence + "\n")
-
+    
             # Display the processed sequences with headers in the text box
             self.sequence_result_text.clear()
             formatted_sequences = [f"{header}\n{sequence}\n" for header, sequence in sequences]
             self.sequence_result_text.setPlainText("".join(formatted_sequences))
-
+    
         except Exception as e:
             # Display an error message to the user
             error_message = f"An error occurred: {str(e)}"
             error_dialog = ErrorDialog(error_message)
             error_dialog.exec()
 
-
-
     def remove_non_nucleotides(self, sequence):
         # Use a regular expression to remove non-nucleotide characters (A, C, G, T)
         return re.sub(r'[^ACGTacgt]', '', sequence)
 
     def perform_msa(self):
         try:
-
             selected_tool = "clustalo" if self.clustal_radio.isChecked() else "mafft"
-
-            # Check if no file is provided
+    
             if not hasattr(self, 'upload_path') or not self.upload_path:
                 self.alignment_result_text.setPlainText("Please select a FASTA file for alignment.")
                 return False
-
-            input_filename = self.upload_path  # Use the selected file path
-
-            # Check if the file is a valid FASTA file
+    
+            input_filename = self.upload_path
+    
             if not is_valid_fasta(input_filename):
                 self.alignment_result_text.setPlainText(
                     "The selected file is not a valid FASTA file. Please provide a FASTA file.")
                 return False
-
-            # Get the selected alignment visualization tool from the ComboBox
+    
             selected_visualization_tool = self.alignment_visualization_combo.currentText()
-
-            # Initialize stdout and stderr
+    
             stdout = ""
             stderr = ""
-
-            # Perform the sequence alignment using the selected tool
+    
             if selected_tool == "mafft":
-                mafft_cmd = ["mafft", input_filename]  # Provide full path to mafft executable if necessary
-                process = subprocess.Popen(mafft_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+                # Execute MAFFT command
+                output_file = self.generate_output_filename(input_filename)
+                subprocess.run(["mafft", input_filename], stdout=open(output_file, "w"))
+                stdout = open(output_file).read()  # Read the output file content
             elif selected_tool == "clustalo":
-                clustalo_cmd = ["clustalo", "-i", input_filename, "--outfmt=fasta"]
-                process = subprocess.Popen(clustalo_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-                
-                stdout, stderr = process.communicate()
-
-            # Check if alignment was successful
+                # Execute Clustal Omega command
+                output_file = self.generate_output_filename(input_filename)
+                subprocess.run(["clustalo", "--infile", input_filename, "--outfmt", "fasta"], stdout=open(output_file, "w"))
+                stdout = open(output_file).read()  # Read the output file content
+    
             if "error" in stderr.lower():
                 self.alignment_result_text.setPlainText("Alignment failed. Check input and tool.")
                 return False
-
-            # Parse the alignment from stdout
+    
             alignment = AlignIO.read(StringIO(stdout), "fasta")
-
-            # Update the alignment result text box with the alignment content
+    
             self.alignment_result_text.setPlainText(str(alignment))
-
-            # Generate the output filename based on the input filename
-            output_file = self.generate_output_filename(input_filename)
-
-            # Save the alignment to the output file
+    
             with open(output_file, "w") as output_handle:
                 AlignIO.write(alignment, output_handle, "fasta")
-
-            # Choose the alignment visualization tool based on the user's selection
+    
             if selected_visualization_tool == 'jalview':
-                # Launch jalview with the alignment file
                 jalview_command = ["jalview", "-open", output_file]
                 subprocess.Popen(jalview_command)
             else:  # Default to seaview
-                # Launch seaview with the alignment file
                 seaview_command = ["seaview", output_file]
                 subprocess.Popen(seaview_command)
-
+    
             return True
-
+    
         except Exception as e:
             self.alignment_result_text.setPlainText(f"Error: {str(e)}")
 
 
     def generate_output_filename(self, input_filename):
         try:
             # Get the base name of the input filename (without the extension)
             base_name = os.path.splitext(os.path.basename(input_filename))[0]
 
             # Construct the output filename by adding "_alignment.fasta" to the base name
             output_filename = f"{base_name}_alignment.fasta"
             return output_filename
         except Exception as e:
-            self.alignment_result_text.setPlainText(f"Error generating output filename: {str(e)}")
+            # Handle the error, e.g., display a message to the user
+            print(f"Error generating output filename: {str(e)}")
             return "alignment.fasta"  # Default to a hardcoded filename if an error occurs
 
     def phylogeny(self, input_file, tool="MrBayes-Bayesian Phylogeny"):
         try:
-            # Use the selected file path
-            input_file = self.phylogen_file_path if not input_file else input_file
-
             # Check if no input file is provided
             if not input_file:
                 self.output_text.setPlainText("Please select an alignment file.")
                 return
-
+    
+            # Get the base name of the input filename (without the extension)
+            base_name = os.path.splitext(os.path.basename(input_file))[0]
+    
             # Check the alignment format and selected molecular type
             if is_protein_alignment(input_file) and self.molecule_type != "Protein":
                 self.output_text.setPlainText(
                     "Error: The selected molecular type must be 'Protein' for protein alignments.")
                 return
-
-            # Check the alignment format and selected molecular type
+    
             if not is_protein_alignment(input_file) and self.molecule_type == "Protein":
                 self.output_text.setPlainText(
                     "Error: The selected molecular type must be 'DNA' for nucleotide alignments.")
                 return
-
+    
             # Check if the provided file is aligned
             if not is_fasta_aligned(input_file):
                 self.output_text.setPlainText(
                     "Error: The provided alignment file is not aligned. Please provide an aligned FASTA or Nexus file.")
                 return
-
+    
             # Create the output folder if it doesn't exist
-            output_folder = "output"
-            if not os.path.exists(output_folder):
-                os.makedirs(output_folder)
-
-            # Use the self.molecule_type variable for molecule type selection
-            molecule_type = self.molecule_type
-
+            output_folder = "SATO_output"
+            os.makedirs(output_folder, exist_ok=True)
+    
             if tool == "fasttree-Maximum Likelihood":
                 # Run FastTree directly on the input FASTA file to generate a tree file
-                base_name = os.path.splitext(os.path.basename(input_file))[0]
                 tree_path = os.path.join(output_folder, f"{base_name}.tree")
-
+    
                 # Define the command as a list of strings
                 command = ["fasttree", "-out", tree_path, input_file]
-
                 subprocess.run(command, check=True, text=True, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
-
+    
             elif tool == "MrBayes-Bayesian Phylogeny":
+                nexus_file_path = os.path.join(output_folder, f"{base_name}.nex")
+    
                 if input_file.endswith(".fasta"):
                     # Load FASTA alignment
                     alignment = AlignIO.read(input_file, "fasta")
-
-                    # Define the output Nexus file path in the output folder
-                    base_name = os.path.splitext(os.path.basename(input_file))[0]
-                    nexus_file_path = os.path.join(output_folder, f"{base_name}.nex")
-
+    
                     # Write the alignment to a Nexus file with the desired format in the output folder
                     with open(nexus_file_path, "w") as nexus_file:
                         nexus_file.write("#NEXUS\n")
                         nexus_file.write("BEGIN DATA;\n")
-                        nexus_file.write(
-                            f"    DIMENSIONS NTAX={len(alignment)} NCHAR={alignment.get_alignment_length()};\n")
-                        nexus_file.write(f"    FORMAT DATATYPE={molecule_type} MISSING=? GAP=-;\n")
+                        nexus_file.write(f"    DIMENSIONS NTAX={len(alignment)} NCHAR={alignment.get_alignment_length()};\n")
+                        nexus_file.write(f"    FORMAT DATATYPE={self.molecule_type} MISSING=? GAP=-;\n")
                         nexus_file.write("    MATRIX\n")
-
+    
                         for record in alignment:
                             nexus_file.write(f"{record.id}\n{record.seq}\n")
-
+    
                         nexus_file.write("    ;\n")
                         nexus_file.write("END;\n")
-
-                    # Assuming the Nexus file is generated in the 'output' folder
-                    nexus_file_path = os.path.join(output_folder, f"{base_name}.nex")
-
+    
                     # Add MrBayes block to the Nexus file with output file paths in the output folder
                     with open(nexus_file_path, "a") as nexus_file:
                         nexus_file.write("\nBEGIN mrbayes;\n")
                         nexus_file.write(f"    set autoclose=yes nowarn=yes;\n")
                         nexus_file.write("    lset nst=6 rates=invgamma;\n")
                         nexus_file.write("    prset statefreqpr=fixed(equal);\n")
                         nexus_file.write(f"    mcmc ngen=10000;\n")
                         nexus_file.write(f"    sumt burnin=250;\n")
                         nexus_file.write("END;\n")
-
-                    # Run MrBayes with the Nexus file in the output folder as input
-                    subprocess.run(["mb", nexus_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-                    tree_path = os.path.join(output_folder, f"{base_name}.nex.con.tre")
-
+    
                 elif input_file.endswith(".nex"):
-                    # Use the provided Nexus file directly
-                    base_name = os.path.splitext(os.path.basename(input_file))[0]
-                    nexus_file_path = os.path.join(output_folder, f"{base_name}.nex")
+                    # Copy the provided Nexus file to the output folder
                     subprocess.run(["cp", input_file, nexus_file_path], check=True)
-                    subprocess.run(["mb", nexus_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-                    tree_path = os.path.join(output_folder, f"{base_name}.nex.con.tre")
-
+    
                 else:
                     raise Exception("Unsupported file format. Please provide a .fasta or .nex file.")
+    
+                # Run MrBayes with the Nexus file in the output folder as input
+                subprocess.run(["mb", nexus_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    
+                tree_path = os.path.join(output_folder, f"{base_name}.nex.con.tre")
+    
             else:
                 raise Exception("Invalid phylogeny tool selected.")
-
+    
             # Visualize the tree with FigTree (assuming a tree file is generated)
             subprocess.run(["figtree", tree_path])
-
-            # Delete input files in the output folder
-            self.delete_files_in_output_folder()
-
+    
             result_message = "Phylogenetic analysis completed. Tree visualization opened in FigTree."
-
+    
             if not input_file:
                 result_message += "\nProvide the alignment in fasta format or mrBayes configuration file (only for mrBayes)"
-
+    
         except Exception as e:
+            # Handle the error, e.g., display a message to the user
             self.output_text.setPlainText(f"Error performing phylogenetic analysis: {str(e)}")
 
 
+
 def main():
     app = QApplication(sys.argv)
     window = SATOApp()
     window.show()
     sys.exit(app.exec())
 
 if __name__ == '__main__':
```

### Comparing `SATO-0.1.5/SATO/about_intro.txt` & `SATO-0.1.6/SATO/about_intro.txt`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/help.txt` & `SATO-0.1.6/SATO/help.txt`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/icons/download.png` & `SATO-0.1.6/SATO/icons/download.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/icons/fasta.png` & `SATO-0.1.6/SATO/icons/fasta.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/icons/file.png` & `SATO-0.1.6/SATO/icons/file.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/icons/logo-no-background.png` & `SATO-0.1.6/SATO/icons/logo-no-background.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/icons/sato.png` & `SATO-0.1.6/SATO/icons/sato.png`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/stylesheet.css` & `SATO-0.1.6/SATO/stylesheet.css`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO/validation.py` & `SATO-0.1.6/SATO/validation.py`

 * *Files identical despite different names*

### Comparing `SATO-0.1.5/SATO.egg-info/PKG-INFO` & `SATO-0.1.6/SATO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATO
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods
 Home-page: https://github.com/clabe-wekesa/SATO
 Author: Clabe Wekesa
 Author-email: simiyu86wekesa@gmail.com
 License: MIT
 Keywords: consensus,alignment,phylogenetics,bioinformatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SATO-0.1.5/setup.py` & `SATO-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for long description
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     LONG_DESCRIPTION = readme_file.read()
 
 setuptools.setup(
     name="SATO",
-    version="0.1.5",
+    version="0.1.6",
     description='Python package that generates consensus sequence from the forward and reverse sequences, performs multiple sequence alignment of the fasta sequences, and generates phylogenetic trees using Bayesian and Maximum Likelihood Methods',
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="MIT",
     author='Clabe Wekesa',
     author_email='simiyu86wekesa@gmail.com',
     url="https://github.com/clabe-wekesa/SATO",
```

