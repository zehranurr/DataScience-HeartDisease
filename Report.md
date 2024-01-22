
## Heart Disase





It is predicted that heart disease, one of the most common diseases in the world, will continue to
be the number one cause of death for a long time. The fact that many of the factors of heart disease
can be prevented or treated is an opportunity to decrease the loss of life as a result of the disease.
For this reason, many studies aimed at detecting the disease by applying algorithmic and statistical
methods to case data have been conducted. The aim of this study is to examine the relationship
between the characteristics determined and the diagnosis of heart attack and to predict the
diagnosis of a heart attack at the maximum level. The values in the data set with 12 qualities and
303 cases were cleared and then analyzes were made. It has been found that the characteristics of
chest pain type, exercise-induced angina, and exercise-induced ST depression have a high rate of
correlation with the diagnosis of a heart attack. Analysis results were visualized and added to the
study. For the diagnosis of heart attack, 4 different algorithms were applied, namely the C4.5
decision tree, k-nearest neighbor, random forest, and SVM, which were successful in other
studies, and their results were compared. The C4.5 decision tree algorithm has been the most
accurate algorithm for predicting heart attack diagnosis. According to World Health Organization (WHO) data,
deaths due to cardiovascular diseases take the first place among all deaths with 30 percent. In our country, 
this rate is around 47 percent [4]. Myocardial infarction (MI), which is one of the coronary artery diseases and popularly called heart attack,
occurs as a result of disruption of blood supply or oxygenation of a part of the heart.
It is a disease. In other words, it is caused by the insufficient amount of blood and therefore oxygen reaching the heart.
When there is not enough oxygen, damage to the heart occurs, and when there is no oxygen for a long time, death occurs in the heart.


### Posing a risk of death or adversely affecting human health
The main causes of this disease, which affects
can be listed as follows [6]:
- Obesity
- Hypertension
- Diabetes
- Cholesterol
- Gender
- Age
- Tobacco use
- Alcohol use
- Family history



      -«Aksi ispat edilene kadar göğüs ağrısı olan her hasta acildir ve mortalitesi yüksektir.»
       Araş. Gör. Dr. Havva ŞEN






Çalışma sonucunda kalp krizini tetikleyen en önemli
beş faktör, büyük tansiyon değeri, diyabet, obezite,
sigara ve küçük tansiyon değeri olarak bulunmuştur.
Taşçı ve Şamlı [11] yaptıkları çalışmada yüzlerce veri
bulunan veri setine çeşitli algoritmalar uygulayarak
kalp hastalığı teşhisi koyma çalışması yapmıştır. 9
farklı veri madenciliği yöntemini WEKA yazılımında
veri seti üzerinde uygulamışlardır. K-NN yönteminin
en başarılı yöntem olduğunu tespit etmişlerdir

Bu çalışmanın amacı, yaş, cinsiyet, göğüs ağrısı tipi,
istirahat kan basıncı, kolesterol değeri, açlık kan
şekeri, istirahat elektrokardiyografik sonuç,
maksimum nabız, egzersize bağlı anjin, egzersize
bağlı ST depresyonu, ST segmenti eğimi ve defekt tipi
niteliklerinin kalp krizi tanısıyla ilişkisini incelemek
ve kalp krizi tanısını maksimum düzeyde doğru
tahmin etmektir. Çalışma kapsamında veri ön işleme
yapılmış ve veriler düzenlenerek analiz edilmiştir.
Analiz sonuçları görselleştirilerek çalışmaya
eklenmiştir. Tanı tahmini için C4.5 karar ağacı, k-en
yakın komşu, rastgele orman, destek vektör
makineleri algoritmaları kullanılmıştır. 


2.2.1. Veri temizleme (Data cleansing)
Veri temizleme, veri analiz işlemleri yapılmadan önce
kesinlikle yapılması gerekilen bir işlemdir. Eksik
verilerin tamamlaması, tutarsızlıkların giderilmesi ve
aykırı değerlerin saptanması için gürültünün
giderilmesi gibi işlemlerden oluşmaktadır [12]. Eksik
verilerin tamamlanmasında şu yöntemler
kullanılabilir [13]:
 Eksik değer içeren kayıtlar silinebilir.
 Eksik değerler yerine ortalama kullanılabilir.
 Eksik değerler yerine medyan kullanılabilir.
 Eksik değerler yerine içinde bulunduğu sınıfın
ortalaması kullanılabilir.
 Eksik değerler yerine regresyon gibi yöntemler
kullanarak en uygun değer kullanılabilir.
Aykırı değerlerin saptanması için ise kullanılan 3
yöntem bulunmaktadır. Bunlar, binning, kümeleme ve
regresyon yöntemleridir. Olabilecek veri
tutarsızlıkları ise dışsal referans kullanarak
giderilebilir [12]. 
----

# What is a Decision Tree?


Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features. A tree can be seen as a piecewise constant approximation.

# Some advantages of decision trees are:

- Simple to understand and to interpret. Trees can be visualized.
- Requires little data preparation. Other techniques often require data normalization, dummy variables need to be created and blank values to be removed. Some tree and algorithm combinations support missing values.

# The disadvantages of decision trees include:

Decision-tree learners can create over-complex trees that do not generalize the data well. This is called overfitting. Mechanisms such as pruning, setting the minimum number of samples required at a leaf node or setting the maximum depth of the tree are necessary to avoid this problem.



 ------------- The Classification algorithm is a Supervised Learning technique that is used to identify the category of new observations on the basis of training data. In Classification, a program learns from the given dataset or observations and then classifies new observation into a number of classes or groups. Such as, Yes or No, 0 or 1, Spam or Not Spam, cat or dog, etc. Classes can be called as targets/labels or categories.
Binary Classifier: If the classification problem has only two possible outcomes, then it is called as Binary Classifier.
Examples: YES or NO, MALE or FEMALE, SPAM or NOT SPAM, CAT or DOG, etc.