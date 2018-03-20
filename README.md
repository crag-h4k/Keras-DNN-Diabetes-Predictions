Exercise of changing the complexity and sturcture of a ANN to increase accuracy of model

While slow due to a very small batch size, 99.48% accuracy was obtain through this model
model.add(Dense(12, input_dim=8, activation='relu'))
model.add(Dense(20, activation='relu'))
model.add(Dense(20, activation='relu'))
model.add(Dense(20, activation='relu'))
model.add(Dense(8, activation='relu'))
model.add(Dense(1, activation='sigmoid'))
model.fit(X,Y, epochs=1000, batch_size=2)
