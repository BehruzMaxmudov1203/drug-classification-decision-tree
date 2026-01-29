# 🚀 **Drug-Tree** — Smart Drug Recommendation Model

> Machine Learning yordamida bemor uchun eng mos dori turini bashorat qiluvchi model.

---

## 🎯 **Loyiha haqida**

Ushbu loyiha Decision Tree va Random Forest algoritmlaridan foydalanib, bemorning quyidagi xususiyatlariga qarab eng mos dori turini aniqlaydi:

* Age (Yosh)
* Sex (Jins)
* BP (Qon bosimi)
* Cholesterol (Xolesterin darajasi)
* Na_to_K (Natriy/Kaliy nisbati)

Model ko'p toifali klassifikatsiya (multiclass classification) muammosini hal qiladi.

---

## 🧠 **Model qanday ishlaydi?**

Datasetdagi matnli ustunlar Label Encoder orqali raqamlashtiriladi. Keyin:

* **Decision Tree** — asosiy model
* **Random Forest** — natijani yaxshilash uchun
* **Cross-validation** — ishonchlilikni tekshirish

---

## 📊 **Daraxt vizualizatsiyasi**

Quyidagi rasm kabi katta va tushunarli qaror daraxti chiziladi:

![Decision Tree](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExcmJpazl0aDhxM3VqMWtoYjZ3Y2h1bzNqYWxsbzA4eGg5M2kxcGo4bSZlcD12MV9naWZzX3NlYXJjaCZjdD1n/3o7aCTfyhYawdOXcFW/giphy.gif)

---

## 🏗 **Texnologiyalar**

* Python
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 📁 **Kod bo‘lagi**

```python
from sklearn.tree import DecisionTreeClassifier
from sklearn.preprocessing import LabelEncoder

encoder = LabelEncoder()
df['Sex'] = encoder.fit_transform(df['Sex'])
df['BP'] = encoder.fit_transform(df['BP'])
df['Cholesterol'] = encoder.fit_transform(df['Cholesterol'])

X = df[['Age','Sex','BP','Cholesterol','Na_to_K']]
y = df['Drug']

model = DecisionTreeClassifier()
model.fit(X_train, y_train)
```

---

## 🔥 **Natijalar**

Model quyidagilarni beradi:

* Classification report
* Confusion matrix
* Decision Tree visualization

---

## 🎬 **Animatsiya — Machine Learning jarayoni**

![ML Animation](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3Z4YDN1YzJ1OXMybWRydXdlZWowczNrbTA1aWlvMGZ4czBpZDFmNiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/LMcB8XospGZO8UQq87/giphy.gif)

---

## 👨‍⚕️ **Maqsad**

Kelajakdagi bemorlarga dori tanlash jarayonini:

* avtomatlashtirish,
* tezlashtirish,
* va aniqroq qilish.
