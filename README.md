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

- Speed (Average): Naver Cloud < Azure < GCP< AWS </div>
- Variability: RTT variabilty(standard deviation): Naver Cloud < Azure < GCP < AWS </div>
- Max RTT: Naver Cloud < Azure < GCP < AWS
## Correlation
|	|AWS_Seoul|	GCP_Seoul|	Azure_Seoul|	Ncloud_Seoul|
|------|---|---|---|---|
|AWS_Seoul|		|0.749633|	0.704170|	0.599486|
|GCP_Seoul|	0.749633|	|	0.870898|	0.747465|
|Azure_Seoul|	0.704170|	0.870898|		|0.766605|
|Ncloud_Seoul|	0.599486|	0.747465|	0.766605| |	
AWS, GCP, Azure, and NAVER exhibit a high correlation in RTT with each other, so it may be more advantageous to use each platform for backup purposes rather than traffic distribution. In particular, the correlation between AWS and NAVER is lower compared to other platform combinations, which suggests that combining these two platforms in a multi-cloud strategy can yield complementary effects.
