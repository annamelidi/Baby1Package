#' Extracting the first plot
#'
#' @param x:an expression matrix
#'
#' @return the boxplot
#' @export
#'

Make_figure_1 <- function(x){

#Read the data (within the package??? -> inst file)

#baby_data <- readr::read_delim("/Users/mimislfc/Desktop/ΑΝΝΑ ΙΙΒΕΑΑ/baby package /baby_data.csv", col_names=TRUE, show_col_types = FALSE )
#readr::write_excel_csv(baby_data, path = "inst/exdata/baby_data.csv")

# baby_data <- readr::read_csv(system.file("exdata", "baby_data.csv", package = "BabyPackage"), show_col_types = FALSE)

 data("baby_data")
View(baby_data)

#Making the plot
figure_1 <- ggplot(baby_data, aes(baby_data$GeneSymbol)) +
  geom_point(aes(y=baby_data$GSM3444310), colour="red") +
  geom_point(aes(y=baby_data$GSM3444311), colour="green") +
  theme(legend.title= element_text("Sample ID"), legend.position = "bottom" )
#Save the plot
png("figure_1.png")
print(figure_1)
dev.off()
}
