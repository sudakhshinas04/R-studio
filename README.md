# R-studio
1+1
library(igraph)
install.packages("igraph")
user_lib <- file.path(Sys.getenv("USERPROFILE"), "Documents", "R", "win-library", "4.6")
dir.create(user_lib, recursive = TRUE, showWarnings = FALSE)
.libPaths(c(user_lib, .libPaths()))
browseURL("https://cloud.r-project.org/src/contrib/PACKAGES")
install.packages("igraph", lib = user_lib, repos = "https://cran.rstudio.com/")
library(igraph)
packageversion("igraph")
package.version("igraph")
x <- read.table("C:/mapping/mi_klnc_nodes.txt",header = TRUE)
print(x)
q()
library(igraph)
library(igraph)
q
library(igraph)
q
q()
library(igraph)
x <- read.table ("C:/mapping/klnc_mapping.txt", header = TRUE)
print(x)
x <- read.table ("C:/mapping/miRNA_mapping.txt", header = TRUE)
print(x)
x <- read.table ("C:/mapping/mrna_mapping.txt", header = TRUE)
print(x)
x <- read.table ("C:/mapping/combined_edgelist.txt", header = TRUE)
print(x)
all_edges <- rbind(x,x,x)
net <-graph_from_data_frame(all_edges, directed = TRUE)
plot(net, vertex.label = NA, vertex.sizes = 5)
view(all_edges)
View(all_edges)
plot(net, vertex.label = NA, vertex.sizes = 2.5)
plot(net, vertex.label = NA, vertex.sizes = 2)
plot(net, vertex.label = NA, vertex.sizes = 2)
plot(g, layout = layout_with_fr, vertex.size = 6, vertex.label.cex = 0.5, edge.arrow.size = 0.3, main = "mRNA-miRNA-lncRNA Interaction Network")
plot(net, layout = layout_with_fr, vertex.size = 6, vertex.label.cex = 0.5, edge.arrow.size = 0.3, main = "mRNA-miRNA-lncRNA Interaction Network")
v(g)$color <- membership(comm)
node_colors <- rep("gray", length(v(net)))
node_colors <- rep("gray", length(v(g)))
node_colors <- rep ("gray", length(v(net)))
node_colors <- rep ("gray", length(V(net)))
node_colors [grep ("URS", V(net)$name, ignore.case = TRUE)] <- "tomato"
node_colors [grep ("OSA-miR", V(net)$name, ignore.case = TRUE)] <- "skyblue"
node_colors [grep ("Os", V(net)$name, ignore.case = TRUE)] <- "green"
V(net)$color <- node_colors
table(V(net)$color)
node_colors [grep ("Os", V(net)$name, ignore.case = TRUE)] <- "green"
node_colors [grep ("URS", V(net)$name, ignore.case = TRUE)] <- "tomato"
node_colors [grep ("OSA-miR", V(net)$name, ignore.case = TRUE)] <- "skyblue"
node_colors [grep ("OSA-miR", V(net)$name)] <- "green"
V(net)$color <- node_colors
table(V(net)$color)
plot(net, layout = lay, vertex.size = 6, vertex.color = V(net)$color, vertex.frame.color = NA, vertex.label = V(net)$name, vertex.label.cex = 0.25, vertex.label.color = "black", vertex.label.dist = 0.3, edge.arrow.size = 0.3, main = miRNA-lncRNA Interaction Network)
plot(net,
layout = lay,
vertex.size = 6,
vertex.color = V(net)$color,
vertex.frame.color = NA,
vertex.label = V(net)$name,
vertex.label.cex = 0.25,
vertex.label.color = "black",
vertex.label.dist = 0.3,
edge.arrow.size = 0.3,
main = "miRNA-lncRNA Interaction Network")
lay <- layout_with_fr(net)
plot(net,
layout = lay,
vertex.size = 6,
vertex.color = V(net)$color,
vertex.frame.color = NA,
vertex.label = V(net)$name,
vertex.label.cex = 0.25,
vertex.label.color = "black",
vertex.label.dist = 0.3,
edge.arrow.size = 0.3,
main = "miRNA-lncRNA Interaction Network")
legend("topleft", legend = C ("URS", "OSA-miR", "OS"), col = C("tomato", "skyblue", "green"),pch=19, pt.cex = 1.5, cex = 0.9, bty = "n")
legend("topleft",
legend = c("URS", "OSA-miR", "OS"),
col = c("tomato", "skyblue", "green"),
pch = 19,
pt.cex = 1.5,
cex = 0.9,
bty = "n")
lay <- layout_with_fr(g)
lay <- layout_with_fr(net)
pdf("miRNA_lncRNA_network.pdf", width = 12, height = 10)
pdf("miRNA_lncRNA_network.pdf", width = 12, height = 10)
png("miRNA_lncRNA_network.png", width = 3600, height = 3000, res = 300, type = "cairo")
while (!is.null(dev.list())) dev.off()
plot(net,
layout = lay,
vertex.size = 5,
vertex.color = V(net)$color,
vertex.frame.color = NA,
vertex.label = V(net)$name,
vertex.label.cex = 0.35,
vertex.label.color = "black",
vertex.label.dist = 0.25,
edge.arrow.size = 0.25,
main = "miRNA-lncRNA Interaction Network")
legend("topleft",
legend = c("URS", "OSA-miR", "OS"),
col = c("tomato", "skyblue", "green"),
pch = 19,
pt.cex = 1.5,
cex = 1.0,
bty = "n")
svg("C:/Users/sudak/OneDrive/Desktop/adv progg/Rplot_defined.svg",
width = 16, height = 13)
plot(net,
layout = lay_clean,
vertex.size = v_sizes,
vertex.color = V(net)$color,
vertex.frame.color = "white",
vertex.frame.width = 0.4,
vertex.label = V(net)$name,
vertex.label.cex = 0.15,
vertex.label.color = "gray15",
vertex.label.dist = 0.4,
edge.color = adjustcolor("gray55", alpha.f = 0.22),
edge.width = 0.5,
edge.arrow.size = 0.2,
main = "miRNA-lncRNA Interaction Network")
plot(net,
layout = lay,
vertex.size = 6,
vertex.color = V(net)$color,
vertex.frame.color = NA,
vertex.label = V(net)$name,
vertex.label.cex = 0.15,
vertex.label.color = "black",
vertex.label.dist = 0.4,
edge.arrow.size = 0.3,
main = "miRNA-lncRNA Interaction Network")
plot(net,
layout = lay_clean,
vertex.size = v_sizes,
vertex.color = V(net)$color,
vertex.frame.color = "white",
vertex.frame.width = 0.4,
vertex.label = V(net)$name,
vertex.label.cex = 0.15,
vertex.label.color = "gray15",
vertex.label.dist = 0.4,
edge.color = adjustcolor("gray55", alpha.f = 0.22),
edge.width = 0.5,
edge.arrow.size = 0.2,
main = "miRNA-lncRNA Interaction Network")
legend("topleft",
legend = c("URS", "OSA-miR", "OS"),
col = c("tomato", "skyblue", "green"),
pch = 19,
pt.cex = 1.6,
cex = 1.0,
bty = "n")
library(pheatmap)
install.packages("pheatmap")
library(pheatmap)
history
savehistory("C:/Users/sudak/OneDrive/Desktop/adv progg/r code.Rhistory")
