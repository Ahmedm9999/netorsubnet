In this assignment we were asked to do calculations on many IP addresses and to check each of the addresses whether it is a NET or SUBNET address, I will also attach the questions of the assignment here in the README and in the file called netorsubnet.TXT you can see the answers accordingly .


# Net or Subnet?

People use the term **"subnet"** too much, even when what they are talking about is not really a sub-network. Use this exercise to make sure you know how to tell real subnet from complete networks.

## The basics (and examples)

Remember network classes:  
- **CLASS A**:   0.0.0.0 - 127.255.255.255
- **CLASS B**: 128.0.0.0 - 191.255.255.255
- **CLASS C**: 192.0.0.0 - 223.255.255.255
- **CLASS D**: 224.0.0.0 - 239.255.255.255 (used for IP MULTICAST)
- **CLASS E**: 240.0.0.0 - 255.255.255.255 (EXPERIMENTAL - NOT USED)  

- Example 1:  
What is 130.1.2.0/24 ?
It is not anything in class C, even if the mask (the /24) matches the default mask of Class C networks.  
You can see that the IP address is within the CLASS B range.  
So, it is a subnet of a class B network.

- Example 2:  
What is 200.1.2.0/24 ?  
This is not a subnet at all !!!  
It is a complete CLASS C network.  
Not a subnet.

- Example 3:  
What is 80.40.0.0/8 ?  
You'll not believe this, but this is not a network nor a subnetwork.  
This is an IP address of a host (i.e. computer), one of the addresses in the 80.0.0.0/8 complete network.

- Example 4:  
What is 203.202.201.6/24 ?  
This is one of the IP addresses of a complete Class C network (203.202.201.0/24)

- Example 5:  
What is 150.0.0.0/8 ?  
This is a block of mant class B networks, not a class A network.

## Copy to your text editor and answer

For each of the following, say if it is a subnet or not, and in what network class:  

- 115.1.0.0/16  
________________________________________________
- 74.0.0.0/8  
________________________________________________
- 199.198.197.196  
________________________________________________
- 222.0.0.0/8  
________________________________________________
- 40.50.30.20/8  
________________________________________________
- 2.0.0.2/16  
________________________________________________
- 172.16.0.0/24  
________________________________________________
- 10.0.0.0/8  
________________________________________________
- 100.100.80.1/8  
________________________________________________
- 6.6.6.6/16  
________________________________________________
- 1.0.0.0/8  
________________________________________________
- 235.235.0.0/24  
________________________________________________________________________________________________________________________________________________

# Partition That

You have received a single CIDR block.  
You have to partition that in the following way:  

- The initial block (we'll call it B):  
**87.87.0.0/18**
  - **Answer**: how many addresses are in this block?
  - **Answer**: what is the broadcast address of the block?
- Split the block into 4 CIDR blocks (let's call them B1, B2, B3, B4)
  - **Answer**: write the network address and the broadcast address of each block.  
  - **Answer**: how many addresses are in each block?
- Split block B3 into 8 networks (let's call them B31,B32,B33,B34,B35,B36,B37,B38) 
- Split B37 into 4 networks (B371, B372, B373, B374)
  - **Answer**: Write the network and broadcast address of each one

# Ahmed Massalha
