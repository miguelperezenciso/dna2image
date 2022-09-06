# Computer generation of fruit shapes from DNA sequence
## Citation:
M. Pérez-Enciso, C. Pons, A. Graell, A.J. Monforte, L.M. Zingaretti. Computer generation of fruit shapes from DNA sequence. Biorxiv. submitted

Code to generate images from dna sequence


### Summary

The generation of realistic plant and animal images from marker information could be a main contribution of artificial intelligence to genetics and breeding. Since morphological traits are highly variable and highly heritable, this must be possible. However, a suitable algorithm has not been proposed yet. This paper is a proof of concept demonstrating the feasibility of this proposal using ‘decoders’, a class of deep learning architecture. We apply it to Cucurbitaceae, the family harboring the largest variability in fruit shape in the plant kingdom, and to tomato. We generate Cucurbitaceae shapes assuming a hypothetical, but plausible, evolutive path along observed fruit shapes. In tomato, we analyze 129 crosses for which image and genotype data were available. In both instances, a simple decoder was able to recover expected shapes with large accuracy. For the tomato pedigree, we also show that the algorithm can be trained to generate offspring images from their parents’ shapes, fully bypassing genotype information.

### Contents


- Generates 2D and 3D ellipses: https://github.com/miguelperezenciso/dna2image/blob/main/dna2img.ellipse.ipynb
- Generates cucurbit shapes: https://github.com/miguelperezenciso/dna2image/blob/main/dna2img.cucurbita.ipynb
- Generates tomato shapes: https://github.com/miguelperezenciso/dna2image/blob/main/dna2img.tomato.ipynb
- Generates 'offspring' ellipses from 'parents' ellipses: https://github.com/miguelperezenciso/dna2image/blob/main/img2img.ipynb
- Generates 'offspring' tomato shapes from 'parents' shapes: https://github.com/miguelperezenciso/dna2image/blob/main/img2img.ipynb

**Warning:** The last code requires file TraditomImageset.pkl (~1Gb), which is available from dropbox link https://www.dropbox.com/s/hvmt1a2qursameq/TraditomImgset.pkl?dl=0

### Some relevant sites / documentation used
- https://docs.opencv.org/master/d6/d00/tutorial_py_root.html
- https://scikit-image.org/
- https://github.com/lauzingaretti/DeepAFS 
- https://machinelearningmastery.com/
- https://machinelearningmastery.com/deep-learning-for-computer-vision/
- Geron A. 2019. https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/
- Chollet F. 2017. https://www.manning.com/books/deep-learning-with-python , p122 ff for CNNs
- https://github.com/Horea94

### Relevant image libraries are
- skimage: basic
- opencv: advanced, classical library 
- PIL: basic operations, saving, rotating: https://pillow.readthedocs.io/en/stable/handbook/index.html

### Required non standard libraries
- pymrt: as downloaded from the web to generate 3D images
- procrustes
