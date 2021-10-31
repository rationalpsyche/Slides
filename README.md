# Slides

## About

Just a ready to use markdown template to put together a pdf slide deck when in a hurry.

## Pre-requisites

`sudo apt install texlive-latex-base texlive-latex-recommended texlive-latex-extra texlive-fonts-extra`

## How to

Checkout submodule

`git clone --recurse-submodules <url>` or `git submodule update --init --recursive` (if already checked out)

Compile style files for the metropolis theme

`cd mtheme && make sty && mv *.sty ../ && cd ..`

Compile template with pandoc, using a custom eisvogel to have small font for code blocks

`pandoc -t beamer slide.txt -o slide.pdf --listings --template=customEisvogel.tex`
