# Clasificación de Enfermedades en Hojas de Banano

## Información del Proyecto
- **Autor**: Gabriel Emilio García Mazón
- **Universidad**: UTMACH - Facultad de Ciencias Agropecuarias
- **Fecha**: 2025-08-31 02:34:26
- **Ruta**: Clasificación con modelos preentrenados (Transfer Learning)

## Problema a Resolver
Clasificar automáticamente enfermedades en hojas de banano para ayudar a agricultores en la detección temprana de patologías que afectan la producción.

## Dataset
- **Fuente**: Dataset local de enfermedades en banano (Data-Tesis únicamente)
- **Clases**: Cordana, Sanas, SigatokaNegra
- **Total de imágenes**: 900
- **División**: Train (630), Val (180), Test (90)

## Modelos Comparados
1. **ResNet50**: Arquitectura residual profunda con skip connections
2. **MobileNetV3-Large**: Optimizado para eficiencia y velocidad
3. **EfficientNet-B0**: Balance óptimo entre precisión y eficiencia

## Métricas Utilizadas
- **Accuracy**: Porcentaje de clasificaciones correctas
- **Precision Macro**: Precisión promedio por clase
- **Recall Macro**: Sensibilidad promedio por clase  
- **F1-Score Macro**: Balance entre precisión y recall
- **ROC-AUC Macro**: Área bajo la curva ROC

## Resultados Principales
**Mejor Modelo**: MobileNetV3 con Accuracy = 0.9444

### Comparación Completa:

#### ResNet50
- Accuracy: 0.9222
- F1-Score: 0.9228
- Velocidad: 3065.6 imgs/seg

#### MobileNetV3
- Accuracy: 0.9444
- F1-Score: 0.9443
- Velocidad: 2248.6 imgs/seg

#### EfficientNet-B0
- Accuracy: 0.9222
- F1-Score: 0.9217
- Velocidad: 1803.2 imgs/seg

## Archivos Generados
- `experiment_results.json`: Resultados completos
- `tabla_comparativa.csv`: Tabla comparativa de métricas
- `metrics_comparison.html`: Gráficos interactivos
- `confusion_matrices.png`: Matrices de confusión
- `training_curves.png`: Curvas de entrenamiento
- `inference_example_*.png`: Ejemplos de clasificación
- `class_performance.png`: Rendimiento por clase

## Cómo Ejecutar
1. Abrir `Proyecto_Clasificacion.ipynb` en Google Colab
2. Seleccionar GPU (T4 recomendada)
3. Ejecutar todas las celdas secuencialmente
4. Los resultados se guardan automáticamente en `/results`

## Aplicación Práctica
- Diagnóstico automático de enfermedades en cultivos
- Aplicaciones móviles para agricultores
- Sistemas de monitoreo de plantaciones
- Detección temprana para prevenir pérdidas

## Dataset Original
- Fuente: https://github.com/NixonJimenez02/deep-learning-banana-diseases
- Solo se utilizó la carpeta Data-Tesis (900 imágenes aprox.)
