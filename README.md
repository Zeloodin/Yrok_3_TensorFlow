1.
Добавление:
MaxPooling2D( (2,2), strides = 2),
      Conv2D(256, padding = 'same', kernel_size = (3,3), activation = 'relu' )

Результат.
1875/1875 [==============================] - 12s 6ms/step - loss: 0.0936 - accuracy: 0.9645 - val_loss: 0.2962 - val_accuracy: 0.9152
CPU times: user 2min, sys: 8.57 s, total: 2min 9s
Wall time: 2min 23s


2.
Изменение:
kernel_size = (3,3)

На:
kernel_size = (6,6)

Результат.
1875/1875 [==============================] - 11s 6ms/step - loss: 0.0844 - accuracy: 0.9675 - val_loss: 0.3400 - val_accuracy: 0.9138
CPU times: user 1min 52s, sys: 8.51 s, total: 2min
Wall time: 2min 23s


3.
Дополнительное изменение с 2:
MaxPooling2D( (2,2), strides = 2)

На:
MaxPooling2D( (4,4), strides = 2)

Результат.
1875/1875 [==============================] - 10s 5ms/step - loss: 0.1396 - accuracy: 0.9471 - val_loss: 0.2754 - val_accuracy: 0.9166
CPU times: user 1min 42s, sys: 8.69 s, total: 1min 51s
Wall time: 1min 44s


4.
Дополнительное изменение с 3;
kernel_size = (6,6), activation = 'relu'

На:
kernel_size = (6,6), activation = 'softmax'

Результат.
1875/1875 [==============================] - 10s 5ms/step - loss: 2.3028 - accuracy: 0.0994 - val_loss: 2.3026 - val_accuracy: 0.1000
CPU times: user 1min 46s, sys: 8.4 s, total: 1min 54s
Wall time: 1min 47s


5.
Изменение:
strides = 2
x_train, y_train_cat, batch_size=32

На:
strides = 4
x_train, y_train_cat, batch_size=64

Результат.
938/938 [==============================] - 5s 5ms/step - loss: 0.2025 - accuracy: 0.9251 - val_loss: 0.2877 - val_accuracy: 0.8941
CPU times: user 54.7 s, sys: 5.01 s, total: 59.7 s
Wall time: 1min 23s


