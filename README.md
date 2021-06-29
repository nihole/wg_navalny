# wg_navalny

This is a wikigraph data repository. 

Wikigraph is a graph created based on principles of Wave Analysis. Refer to https://github.com/nihole/wikigraph/ for details.

# What is investigated

The statement under investgation is

**"Was Alexei Navalny poisoned by the Russian special services or not?"**

So the root node's statement is 

**"This (poisoning) was an operation by the Russian special services."**

# Folders structure

- **yaml**. This is where the YAML files are located, describing the logical chains (waves) 
  - **kremlin**. This data is related to the Kremlin's line of defense. This is the point of view offered and cultivated by the Russian authorities
  - **nw_1**. We took only one statement of Russian authorities and analyzed it using wave analysis. nw_1 stands for negative wave 1 and is related to node with id = '--1--' and the statement "Who needs him?" (Putin)
  - **draft**. These are just experimental graphs. Pay no attention to it
- **graphs**. This folder is used for graphs. These graphs are created from previously discussed YAML files (refer to https://github.com/nihole/wikigraph/ for details) 
  - **kremlin**. Graph [kremlin_navalny.svg](https://github.com/nihole/wg_nav/blob/main/graphs/kremlin/kremlin_navalny.svg) is created from [kremlin_navalny.yml](https://github.com/nihole/wg_nav/blob/main/yaml/kremlin/kremlin_navalny.yml) YAML file
  - **nw_1**. Graph [nw_1.svg](https://github.com/nihole/wg_nav/blob/main/graphs/nw_1/nw_1.svg) is created from [nw_1.yml](https://github.com/nihole/wg_nav/blob/main/yaml/nw_1/nw_1.yml) YAML file

# Results

This analysis is still ongoing. At the moment we have two more or less complete subtrees associated with:

- Kremlin point o view (Kremlin defense)

<img src="https://github.com/nihole/wg_nav/blob/main/graphs/kremlin/kremlin_navalny.svg" alt="Kremlin deffense">

- Analysing of only one statement in this Kremlin defence: "Who needs him?" (Putin)

<img src="https://github.com/nihole/wg_nav/blob/main/graphs/nw_1/nw_1.svg" alt="Who needs him?">

Click on the images above and select "Raw" on the right side of the panel above the image (without this, the node links won't work). Then, by navigating to the nodes of the graph and clicking on the links, you will open wiki articles related to node descriptions.
