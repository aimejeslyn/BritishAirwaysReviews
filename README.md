# BritishAirwaysReviews

**Practicing Data 
source code: https://www.kaggle.com/code/minnikeswarrao/sentiment-analysis**

<img width="568" alt="image" src="https://github.com/aimejeslyn/BritishAirwaysReviews/assets/91269730/579d8a87-1a58-45db-8acc-3ed6c165f08d">

**Graph Rating**

cols=['seating_comfort','staff_service','food_quality','value_for_money']

y=[data[i].mean() for i in cols]
graph2=plt.bar(cols,y,color=['Green','Yellow','Blue','cyan'],edgecolor='black')
for bar in graph2:
    height= bar.get_height()
    plt.annotate(round(height,2),(bar.get_x()+bar.get_width()/2,height/2),ha='center',color='black',fontsize=15)
plt.ylim(0,5)
plt.title('Quality Ratings')
plt.ylabel('Average Rating')
plt.savefig('Quality_Ratings.jpg')
plt.show()

<img width="293" alt="image" src="https://github.com/aimejeslyn/BritishAirwaysReviews/assets/91269730/54772584-0ee8-4ce9-95b6-11d15244eeab">

**Sentiment Analysis**
fig=plt.figure()
fig.set_figwidth(10)
fig.set_figheight(10)
plt.pie(counts.values,labels=counts.index,autopct='%1.1i%%',textprops={'fontsize':15})
plt.title('Sentiment Analysis',fontsize=25,color='red')
plt.savefig('Sentiment_Analysis.jpg')
plt.show()
![Uploading image.png…]()

