# BubbleDB
BubbleDB is a **fictional** and an innovative 3D database system inspired by the fluid dynamics of bubbles in a fluid, akin to those seen in effervescent drinks. In this database, data is represented as bubbles, which can be visualized and interacted with in a three-dimensional space. This unique approach offers an intuitive and efficient way to manage and access data.

# Features

 - 3D Data Representation: Data is visualized as bubbles in a 3D space, offering a unique perspective on data storage and interaction.
 - Multi-dimensional Data Representation: In addition to 3D, BubbleDB supports a 4D view (including time as a dimension) to visualize changes in data over time.
 - Customizable Bubble Shapes: Bubbles can be round, hexagonal, or other shapes, optimizing read and write operations.
 - Customizable Bubble Textures and Colors: Bubbles can have different textures and colors, representing different types of data or data states (e.g., encrypted, public, private).
 - Flexible Positioning and Sizing: Bubbles are positioned in a 3D space using coordinates (x, y, z) and can be specified in mm, cm, in, pixels, bits, or bytes. Bubble sizes can vary and are specified in bytes, bits, liters, etc., reflecting the amount of data they contain.
 - Dynamic Data Access Optimization: Frequently accessed bubbles are automatically moved closer to the "surface" for quicker access, mimicking the behavior of rising bubbles in a fluid.
 - Intelligent Data Clustering: Bubbles naturally cluster based on data relationships, similarities, or user-defined parameters, facilitating easier data correlation analysis.
 - Sectional Data Reading: Reading data within a bubble is dependent on its shape, allowing for optimized data retrieval methods based on bubble geometry.
 - Comprehensive API: Includes functions for reading, writing, deleting, moving, and accessing specific sections of bubbles and within bubbles.
 - Predictive Analytics Engine: Powered by advanced machine learning algorithms, the engine analyzes current and historical data to forecast future outcomes, filling the future-state bubbles with predictive data.

# API Reference

```
createBubble(data, shape, size, location): Creates a new bubble with specified data, shape, size, and location.
readBubble(location): Retrieves data from a bubble at a given location.
readSection(location, sectionParameters): Reads a specific section within a bubble, with parameters tailored to the bubble's shape.
updateBubble(location, newData): Updates the data in a bubble at a specified location.
deleteBubble(location): Deletes a bubble at a given location.
moveBubble(currentLocation, newLocation): Moves a bubble from one location to another.
analyzeBubblePatterns(patternParameters): Analyzes and reports on patterns and correlations among bubbles.
encryptBubble(location, encryptionParameters): Encrypts data within a bubble for enhanced security.
mergeBubbles(locations): Merges multiple bubbles into one, combining their data.
splitBubble(location, splitParameters): Splits a bubble into multiple smaller bubbles based on specified parameters.
```

# Sectional Reading

Depending on the shape of the bubble, the method to locate and read specific sections of data within the bubble varies:

 - Round Bubbles: Utilize spherical coordinates (radius, polar angle, azimuthal angle) to pinpoint data sections.
 - Hexagonal Bubbles: Employ a grid-based system aligned with the hexagon's geometry for segmenting and accessing data.

# Installation

```
git clone https://github.com/23ewrdtf/BubbleDB.git
cd BubbleDB
pip install -r requirements.txt
```

# Usage

```
python
from bubble_db import BubbleDB

db = BubbleDB()
db.createBubble(data="Hello, World!", shape="round", size="10 bytes", location=(1,2,3))
print(db.readBubble((1,2,3)))
print(db.readSection((1,2,3), sectionParameters={'radius': 0.5, 'angle': 30}))
```

# Visual Database Navigation

 - Interactive 3D Visualization: Users can interact with the database in a 3D space, visually navigating through data bubbles.
 - Real-Time Data Interaction: Enables real-time manipulation of data bubbles, including repositioning, resizing, and accessing data.
 - Enhanced Data Understanding: Provides a novel way to understand the structure, relationships, and access patterns of data in the database.
