[< Voltar](/README.md)


## Seleção de Modelo
Modelos maiores como YOLOv5x e YOLOv5x6 produzirão melhores resultados em quase todos os casos, mas têm mais parâmetros, requerem mais memória CUDA para treinar e são mais lentos para executar. Para implantações móveis, recomendamos YOLOv5n, YOLOv5s ou YOLOv5m, para implantações em nuvem, recomendamos YOLOv5l ou YOLOv5x

![image](https://user-images.githubusercontent.com/20934770/153324590-56bf01c8-88ee-49a8-b09a-750f8bc1e46f.png)

## Configurações de treinamento

Epochs: Se o overfitting não ocorrer após 200 épocas, treine por mais tempo.
ImageSize: conjuntos de dados personalizados serão beneficiados treinamento em resolução nativa ou superior. Os melhores resultados de inferência são obtidos no mesmo tamanho em que o treinamento foi executado, ou seja, se você treinar com tamanho 1280, você também deve testar e detectar com 1280.
Batch: Use o maior batch permitido pelo seu hardware. Tamanhos de batchs pequenos produzem estatísticas ruins e devem ser evitados.
