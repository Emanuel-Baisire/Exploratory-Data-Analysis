#Reads data from a local directory

data<- read.table("~/twitter/household_power_consumption.txt", header=TRUE, nrows=2100000, sep=";", stringsAsFactors =FALSE)

#Creates a subset to generate data related to the specified date period

subset<- data[data$Date %in% c("1/2/2007","2/2/2007") ,]

#Generates Plot1

png("plot1.png", width = 480, height = 480)

hist(as.numeric(subset$Global_active_power), col="red",main = "Global Active Power",xlab="Global Active Powe(kilowatts)")

dev.off()
