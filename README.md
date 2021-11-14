# Fault Segmentation on Seismic Data Using CNNs
Mapping fault planes using seismic images is a crucial and time-consuming step in hydrocarbon prospecting.
Conventionally, this requires significant manual efforts that normally go through several iterations to optimize how the different fault planes connect with each other.​  
 Many techniques have been developed to automate this process, such as seismic coherence estimation, edge detection, and ant-tracking, to name a few. 
However, these techniques do not take advantage of the valuable experience accumulated by the interpreters. ​ 
Using CNNs, however, is a technique to automatically detect and map fault zones using 3D seismic images in a similar fashion to the way done by interpreters.
### Dataset
> The training data consisted of **200 synthetic seismic volumes** and corresponding volumes containing fault labels.
> The validation data consisted of another 20 synthetic seismic volumes with corresponding volumes containing fault labels.
> 
> The training dataset was further expanded by inclusion of 5 seismic sections from [F3 dataset from the Netherlands](https://terranubis.com/datainfo/F3-Demo-2020).
> 
>![tiles](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/1.png)
>
> The labels for the seismic section were created manually using adobe illustrator.
>![tiles](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/1f.png)
>
> Finally, 10,000 tiles(128x128) were created from these 5 seismic sections and included into the dataset.
>![tiles](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(258).png)

### Model
>Our problem required a **simplified U-net**.
>

### Accuracy
>Several models were trained.
>To further increase the accuracy of the model, 5 inline sections from F3 dataset from the Netherlands were taken at random. 
>Fault labels were created manually and each section was broken into a (128x128) tile and fed into the model.
>Resultant training dataset, including the synthetic dataset, consisted of **86800** different seismic sections with their corresponding labels.
>As a result, accuracy furthur increased.
>Final Accuracy of the model: **89.21%** 
>![Accuracy](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(256).png)

### Results
>The model was tested on an actual seismic dataset.
>![Results 1](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(252).png)
>![Results 2](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(253).png)
>![Results 3](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(254).png)
>![Results 4](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Screenshot%20(255).png)

### Process at  a glance
>![Process](https://github.com/PranjalGhildiyal/Fault-Segmentation-on-Seismic-Data-Using-CNNs/blob/main/Process.png)





