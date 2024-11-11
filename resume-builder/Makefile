# Define variables
TEX = xelatex
SRC = resume.tex  # Change to your LaTeX source file name
OUT_DIR = home/static  # Specify the output directory
OUT = resume.pdf  # Desired output PDF file name with directory

# Default target
all: $(OUT)

# Compile the LaTeX document
$(OUT): $(SRC) resume.cls
	$(TEX) $(SRC)
	$(TEX) $(SRC)  # Run it twice to resolve references and TOC

# Clean up auxiliary files
clean:
	rm -f *.aux *.log *.out *.toc *.pdf

# Install dependencies (optional, if necessary)
install:
	sudo apt update
	sudo apt install -y make texlive texlive-xetex texlive-fonts-extra
