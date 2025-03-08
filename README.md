/*Name this external file gallery.js*/

function upDate(previewPic){
    // Get the div with id = "image"
    var imageDiv = document.getElementById("image");
    
    // Change the background image to the source file of the preview image
    imageDiv.style.backgroundImage = "url('" + previewPic.src + "')";
    
    // Change the text to the alt text of the preview image
    imageDiv.innerHTML = previewPic.alt;
}

function unDo(){
    // Get the div with id = "image"
    var imageDiv = document.getElementById("image");
    
    // Revert the background image to the original image
    imageDiv.style.backgroundImage = "none";
    
    // Revert the text to the original text
    imageDiv.innerHTML = "Hover over an image below to display here.";
}
