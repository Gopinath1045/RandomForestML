# RandomForestML

DT

from sklearn.ensemble import RandomForestClassifier
from sklearn.tree import DecisionTreeClassifier
Dclassifier = DecisionTreeClassifier(criterion = 'gini', random_state = 50)
Dclassifier.fit(X_train, y_train)

pred=Dclassifier.predict(X_test)
from sklearn.metrics import accuracy_score
accuracy_score(y_test, pred)


from sklearn import tree
plt.figure(figsize=(15,10))
tree.plot_tree(Dclassifier,filled=True)

