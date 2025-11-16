
## 🌡️ XML → SVG Animated Temperature Graph

A small project that transforms meteorological data written in XML into an animated SVG graph using XSLT.
The goal is to visualize city temperatures in a simple, dynamic, and browser-friendly way.

## 📁 Project Structure
File	Description
meteo2.xml	Contains the list of cities and their temperatures.
meteo2.xsl	XSLT stylesheet that converts the XML data into an animated SVG bar chart.

## 🎨 What the XSLT Generates

✔️ SVG bar chart
✔️ Each bar = one city
✔️ Height = temperature
✔️ Simple animation using <animate>
✔️ Fully generated from the XML data

## 🚀 How to Use
## 1️⃣ Preview directly in the browser
Add this at the top of meteo2.xml:

<?xml-stylesheet type="text/xsl" href="meteo2.xsl"?>


Then open the XML file with Firefox or run a small server and open the file through it:

python -m http.server

## 1️⃣ Preview directly in the browser

Add this at the top of meteo2.xml:

``<?xml-stylesheet type="text/xsl" href="meteo2.xsl"?>``


Then open the XML file with Firefox or run a small server and open the file through it:

``python -m http.server``

# 2️⃣ Generate a standalone SVG file

If you prefer to export the final graph:

``xsltproc -o meteo.svg meteo2.xsl meteo2.xml``


You can then open ``meteo.svg`` in any browser.

## 🎯 Purpose of the Project

This mini-project demonstrates how to:

Structure data using XML

Transform XML with XSLT

Produce graphics using SVG

Apply basic SVG animations without JavaScript

Perfect for academic work, XML/XSLT exercises, or simple data visualization demos.

