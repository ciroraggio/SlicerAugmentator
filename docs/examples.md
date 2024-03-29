<center><h2>SlicerAugmentator</h2></center>

<style>
.navbar {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

.navbar li {  /* Target nested elements within the navbar */
  float: left;
}

.navbar li a {  /* Target links within the navbar */
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change the link color to #111 (black) on hover */
li a:hover {
  background-color: #111;
}
</style>

<ul class="navbar">
  <li><a href="https://ciroraggio.github.io/SlicerAugmentator/index">Home</a></li>
  <li><a href="https://ciroraggio.github.io/SlicerAugmentator/examples">Examples</a></li>
  <li><a href="https://ciroraggio.github.io/SlicerAugmentator/changelog">Changelog</a></li>
  <li><a href="https://ciroraggio.github.io/SlicerAugmentator/developers">Developers</a></li>
</ul>

## Examples
Apply augmentation to your medical image dataset in a few simple steps:

**1.** Choose the path of your images

**2.** Specifies by what name or substring of the name SlicerAugmentator can recognize images (CT, CT.nrrd, .nrrd)

**3.** If you also want to include masks/segmentations associated with the images, simply indicate the name or a substring of the name with which SlicerAugmentator can recognize them (mask, mask.nrrd, _label)

**4.** Indicates what type of hierarchy the images respect. This will allow SlicerAugmentator to maintain the original dataset hierarchy when saving. There are two options: **hierarchical** (use this setting if your images are grouped by case and each case is a folder) or **flat** (use this setting if your images/masks are in a single folder and the case name matches the file name)

<center>            
<img src="https://raw.githubusercontent.com/ciroraggio/SlicerAugmentator/main/assets/SlicerAugmentatorInputExample.png">
</center>

**5.** Choose where you want to save the augmented samples
**6.** Enable as many transformations as you want by specifying parameters for each transformation
<table>
    <tr>
        <td>
            <img src="https://raw.githubusercontent.com/ciroraggio/SlicerAugmentator/main/assets/SlicerAugmentatorEnableTransformsExample1.png">
        </td>
        <td>
            <img src="https://raw.githubusercontent.com/ciroraggio/SlicerAugmentator/main/assets/SlicerAugmentatorEnableTransformsExample2.png">
        </td>
    </tr>
</table>

**7.1** Use the **Preview** button if you want to preview the final result on the first sample of the dataset directly into the Slicer scene, if you are not satisfied, change the parameters and request a new preview

![filled](https://raw.githubusercontent.com/ciroraggio/SlicerAugmentator/main/assets/SlicerAugmentatorScreen.png)

**7.2** If you are satisfied with the result, use the **Run** button to save the augmented samples in the folder chosen in step 5. The files will be saved respecting the input hierarchy, as in this case:

![output_folder](https://raw.githubusercontent.com/ciroraggio/SlicerAugmentator/main/assets/SlicerAugmentatorOutputExample.png)