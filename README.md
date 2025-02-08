# Image-Comparator-MSE-and-SSIM-python
На примере двух изображений:

Первое

![RandomRainbow](https://github.com/user-attachments/assets/799ac376-c656-4079-bf76-3cf1c8b56850)

Второе

![20241101_021513](https://github.com/user-attachments/assets/7006d4e1-d6e6-44df-a37c-b234b6f9d5fe)

Давайте объясню результаты, которые мы получили:

Размеры изображений:

***Shape of Image 1: (800, 800, 3): первое изображение (например, шумовая картина) имеет размеры 800x800 пикселей с 3 цветными каналами (RGB).
    Shape of Image 2: (1836, 3264, 3): второе изображение (например, другое изображение) имеет размеры 1836x3264 и также 3 цветных канала.
    Resized Image 2 Shape: (800, 800, 3): второе изображение было изменено до размера 800x800, чтобы совпадать с первым.

Минимальные размеры:

    Minimum Height: 800, Minimum Width: 800: оба изображения имеют минимальные размеры 800x800, что позволяет выполнять вычисления для SSIM.

Размер окна:

    Using window size: 11: размер окна для вычисления SSIM установлен на 11. Это число указывает, что SSIM будет рассчитываться на основе 11х11 пикселей.

Показатели сравнения:

    MSE: 24727.033571901677: Средняя квадратичная ошибка (MSE) — это мера разницы между двумя изображениями. Меньшее значение MSE указывает на то, что изображения больше схожи, а значение в 24727 указывает на то, что существует заметная разница между ними.
    
    SSIM: 5.795766967194399e-05: Индекс структурного сходства (SSIM) - это мера воспринимаемого сходства между двумя изображениями. Значение SSIM колеблется от -1 до 1, где 1 указывает на полное совпадение. Значение 5.8e-05 (то есть 0.00005796) гораздо ниже 1 и говорит о том, что изображения очень сильно различаются.
    
Интерпретация результатов

    Сравнение: Результаты указывают на то, что два изображения (цветной шум и другое изображение) имеют значительное различие. Можете ожидать получить более низкие значения для MSE и SSIM, если вы сравниваете изображения, которые более схожи по содержимому.
    
    Проверьте данные: Если вам требуется исследовать качество изображений или улучшить их, вы можете попробовать понять, как они были созданы, или использовать другие алгоритмы обработки.
