# Comepare of RTT from my destop to major CSP
Generally, cloud platforms are chosen in the order of AWS, Azure, and GCP, as they are widely used and well-validated. However, there are questions about whether this selection criterion is always the best. The need for selection criteria based on actual performance data is being emphasized.
So I started my research because I was curious about the network latency from my desktop to major cloud platforms such as AWS, GCP, Azure, and Ncloud.

# Enviornment
- OS: Window11
- Network: 1Gbps Cable
- tool:Pyton3.8
<br>

# Result
I collected the data for 7days.
![image](https://github.com/user-attachments/assets/6a563654-c395-4fb0-b3b6-2cebf540bcb9)

|Platform|Average RTT(ms)|Std RTT(ms)|Max RTT(ms)|Min RTT(ms)|
|------|---|---|---|---|
|AWS_Seoul|285.85|176.80|1011.54|60.88|
|GCP_Seoul|191.66|122.21|677.50|58.38|
|Azure_Seoul|119.99|66.15|371.69|37.55|
|Naver_Seoul|63.68|31.35|177.52|14.05|

Speed: Average RTT: Naver Cloud < Azure < GCP< AWS 
</div>
Variability: RTT 변동성(표준편차): Naver Cloud < Azure < GCP < AWS
Max RTT: Naver Cloud < Azure < GCP < AWS
