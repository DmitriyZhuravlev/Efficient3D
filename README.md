# Towards Real-time 3D Object Detection through Inverse Perspective Mapping

**Dmitriy Zhuravlev**
T. Shevchenko National University, Kiev 01601, Ukraine
Email: dzhuravlev@ukr.net
LinkedIn: [Dmitriy Zhuravlev](https://www.linkedin.com/in/dmitriy-viktorovich-zhuravlev/)

## Abstract
3D object detection in road scenes is crucial for computer vision applications. While traditional 2D object detection has seen remarkable success, 3D object detection is still an active area of research. This paper presents an efficient method for monocular 3D object detection using inverse perspective mapping.

The proposed method differs from other approaches that rely on deep learning techniques to estimate an object’s orientation. Instead, it uses geometric constraints to lift 2D detections to 3D. The method utilizes instance segmentation and derived object dimensions to achieve 3D localization by employing inverse perspective mapping. The method successfully combines these elements to determine the object’s position in 3D space accurately. By doing so, it achieves execution speeds and localization errors comparable to pure 2D methods, while also offering the advantages of 3D detection.

This work defines real-world scenarios such as for roadside surveillance cameras and onboard cameras, for which high accuracy and speed of 3D localization can be guaranteed by the proposed algorithm.

## Keywords
3D object detection, inverse perspective mapping, instance segmentation

## Introduction
In recent years, the development of autonomous driving and surveillance systems has led to increased interest in 3D object detection in road scenes. While traditional 2D object detection methods have achieved remarkable success, they are limited in their ability to localize objects in 3D space accurately. As a result, 3D object detection has become an active area of research.

While special equipment-based methods such as LiDAR scanners and RGB-D cameras provide direct 3D object reconstruction, their high cost makes them less accessible. In contrast, monocular camera-based methods are more cost-effective and offer greater flexibility in their setup. However, a major limitation of monocular cameras is that they only provide observations in the plane of a two-dimensional image and do not directly measure the distance to objects.

Despite the progress made in the field, there are still several challenges to be addressed. One of the main limitations of current monocular 3D detection methods is the lack of accurate depth estimation, which can result in inaccurate 3D localization. Moreover, these methods require large amounts of annotated training data and heavy computational resources to execute. Addressing these limitations is crucial to improve the practical applicability of monocular 3D detection methods.

In this article, a novel approach to 3D object detection in road scenes using Inverse Perspective Mapping (IPM) is presented. Unlike other methods that rely on deep learning techniques to estimate object orientation and sizes, the proposed method uses geometric constraints. By utilizing IPM, we can transform the perspective view of a scene into a top-down Bird’s-Eye View (BEV). This transformation enables us to compute the projection of an object in BEV space accurately using its dimensions, classification, and 2D bounding box. This approach allows us to accurately detect objects in 3D spaces with almost no performance loss compared to 2D.

## Conclusion and Implications for Computer Vision Applications
In conclusion, I proposed a novel approach for real-time 3D object detection in autonomous driving scenarios and for traffic cameras, which significantly outperforms current state-of-the-art methods in execution speed at the same level of accuracy. The proposed approach combines inverse perspective mapping, instance segmentation, and geometric classification, and achieves a mean Average Precision (mAP) of 84.5%. It is important to note that while YolactEdge is a powerful and effective instance segmentation method, future advancements in instance segmentation techniques may offer even better performance. The proposed method can be adapted to incorporate newer methods as they emerge, ensuring that it stays at the forefront of instance segmentation capabilities and further enhances the accuracy and efficiency of the 3D detection process.

The implications of my work for computer vision applications are significant, as it provides a more efficient solution for real-time 3D object detection. This is crucial for ensuring safety and reliability in road traffic environments. By enabling timely and accurate detection of objects, the method enhances the overall performance of autonomous driving systems, promotes effective decision-making, and contributes to the overall efficiency of the transportation infrastructure.

## Acknowledgments
I would like to thank the authors of YolactEdge for providing their implementations publicly available, whose code was used for segmentation as an intermediate step of the proposed method.
