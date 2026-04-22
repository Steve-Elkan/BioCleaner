# BioCleaner
A Java-based desktop application for bioinformatics data processing and analysis, featuring CSV cleaning, statistical analysis, and DNA sequence utilities with an interactive Swing UI.

Overview
BioCleaner+ is a mini bioinformatics toolkit designed to:
Clean and preprocess CSV datasets
Perform statistical analysis on biological data
Analyze DNA sequences from FASTA files
The application uses a tabbed interface with JTable visualization, making it suitable for both learning and demonstration purposes.

Features
CSV Cleaner
Load and display CSV files in a table
Remove rows with missing or invalid values
Trim whitespace automatically
Detect and highlight outliers
Display number of rows and columns
Fill missing numeric values with mean (optional)

Statistics Module
Column-wise statistical analysis
Automatically detects numeric columns
Computes:
Mean
Median
Standard Deviation
Minimum and Maximum
Missing values count

Sequence Tools (FASTA)
Load FASTA files
Sequence validation
GC content calculation
Reverse complement
Transcription (DNA to RNA)
Translation (DNA to protein using full codon table)
ORF (Open Reading Frame) detection
Motif search and highlighting
GC-rich region visualization
Project Structure


bioCleanerPlus/
 ├── src/com/biocleaner/
 │   ├── MainApp.java
 │   ├── ui/MainUI.java
 │   ├── csv/
 │   ├── cleaning/
 │   ├── stats/
 │   ├── fasta/
 │   └── sequence/


Requirements
Java JDK 8 or higher
Compatible with Windows, macOS, and Linux
How to Run

Option 1: Run using JAR
java -jar BioCleanerPlus.jar

Option 2: Compile manually
javac -d . $(find src -name "*.java")
java com.biocleaner.MainApp


