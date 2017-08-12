# wmt_ds_conf2017

Notes from 4th Annual Walmart Data Science Conference in Sunnyvale, Jun 23, 2017.

## Trends and Developments in Deep Learning

*Rajat Monga, Google Brain*

common platform for ml

python, R, c++, java

tensor flow models

cucumber sorter in japan

### usage at google  
speech recognition  
vision  
google photos   

identify characters, house numbers  
to use for business     
project sunroof    

medical imaging  
using similar model for detecting in retinal images

ml for robotics  
combine vision with robotics

smart reply  

translation  
scale issues  

combine vision and language  
google translate  point to image   

ranking  

recommendation: retrieval + ranking

memorization + generalization

wide & deep  
zero-shot

bigger models but sparsely activated  

automated ml - learn to learn

deep learning is transforming how we design computers  
reduced precision ok   
==> TPU: Tensor processing Unit  
custom chip for NN computations  
Cloud TPU  

deep neural networks  

qa:  
dl issues around training  

even structured data can use dl

dl success  
combination of data and computation, e.g. gpu.  
simplify feature engineering  

tl optimized for mobile

quantum computing vs dl  

offline auc vs online  
estimate not accurate  
change model  

mobile ml  
latency, e.g. translate app  
offline, dictate  
10s MBs
trading accuracy for computing  

start as simple as possible  model  

fraud detection  
explain to user  
research field

less data, more feature engineering

## Use of Ensemble Learning to create purchase propensity score for recurrent Sam’s buyers, Sudipto Pal

sams member engagement campaigns  
1 billion combinations of member and item  
--> personalization engine  

personalized campaign vs broad reach campaign  
hard coded rules vs calibrate using ml  
under performance   

propensity score --> offer assignment

boosting vs bagging  
learn sequentially vs learn parallelly   
gradient boosting vs random forest  

gbm feature creation:  
member, time, item

##  Small Boxes Big Data: A Deep Learning Approach to Optimize Variable Sized Bin Packing, Feng Mao

deep learning avoids feature engineering  
auto feature selection

prefix based initial clustering to speed up slow Monte carlo

operation heuristics to algorithm heuristics

average order for wmt is 2 items.

Boxes Items pair  
checkout  info to shipping  
sub optimized solution in a short time.

##   Algorithmic Pricing for US Store Investment Initiative, Peibei Shi

smart pricing  

loss of profit, lift of sales  

affinity score = P(B|A)/P(B/not A)

same order and high affinity score

DF: demand forecast

Item Elasticity: variation of quantity over price

    dQ/Q = r dP/P

assumption: Elasticity is constant.

line Elasticity  
aggregated Elasticity

## Ranked constraint reconciliation for price optimization, Jagdish Ramakrishnan

business logic transform. price bounds

constraint set  
violate low priority constraints first, high priority next

slack variable  

## Optimizing WMX Campaign Audience, Peng Yang

WMX: Walmart Exchange

ROAS: return on ad spend  

target item set, Campaign period, budget

single model vs multiple models

item, customer, time  

exponential time decay

post impression sales

## Cooperate and compete - internal auction for cooperative marketing, Tao Zhu

SEM: paid search marketing  
cooperative marketing

tourism destination marketing  
intel inside. lenovo also brand for intel.

keyword ads  on google   

contract based  
not allowed to share one keyword to multiple sponsors

compete for high performance keywords

optimization run daily  

## Retargeting Existing Customers Using Display Ads, Vivek Kaul  

user scoring module  
user recommendation module  

experian data to connect wmt user to facebook user  
id mapping service   

mobile ad --> purchased through desktop


