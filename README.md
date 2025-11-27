# R-PROJECT-S-HUB
📊 Social Network Analysis with R
This repository demonstrates Social Network Analysis (SNA) using the igraph package in R. It covers graph creation, visualization, network measures, and community detection with practical examples.

🚀 Features
Create simple undirected and directed graphs

Visualize networks with custom colors, sizes, and layouts

Compute key network measures:

Degree (in/out/all)

Diameter

Edge density

Reciprocity

Closeness, betweenness, and edge betweenness

Import data from CSV files to build networks

Generate histograms of node degrees

Apply different layouts (Fruchterman-Reingold, Kamada-Kawai)

Identify hubs and authorities

Perform community detection using edge betweenness clustering

📦 Requirements
R (≥ 4.0)

igraph package

Install igraph with:

r
install.packages("igraph")
📂 Usage
Clone this repository:

bash
git clone https://github.com/your-username/social-network-analysis.git
Open the R script in RStudio or your preferred IDE.

Run the code step by step to:

Create sample graphs

Import your own CSV data

Visualize networks

Analyze network properties

📑 Example Code
r
library(igraph)

# Create a simple undirected graph
g <- graph(c(1,2,3,3,4,4,5,2,5,4,2,1), directed = FALSE, n=7)
plot(g, vertex.color="green", vertex.size=40, edge.color="red")

# Directed graph with names
g1 <- graph(c("Ram","Arjun","Karan","Udhistir","Ram","Karan"), directed=TRUE)
plot(g1, vertex.color="green", vertex.size=45, edge.color="red")

# Network measures
degree(g1, mode="all")
diameter(g1, directed=FALSE)
edge_density(g1)
📊 Outputs
Graph visualizations with custom layouts

Histograms showing node degree distribution

Hub and authority plots

Community detection diagrams

📁 Data
The script reads a CSV file with two columns (first, second) representing edges between nodes:

csv
first,second
A,B
B,C
C,D
🧩 Community Detection
The project uses edge betweenness clustering to identify densely connected groups within the network.

🎯 Applications
Social media analysis

Citation networks

Organizational structures

Communication patterns

📜 License
This project is licensed under the MIT License – feel free to use and modify.
