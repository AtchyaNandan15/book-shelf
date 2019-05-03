# book-shelf

var book = [
    {
        title: "The Hate u give",
    author: "Angie Thomas",
    stars: 4 
    
    },
    
    {title: "Just listen ",
    author: "Sarah Dessen", 
    stars: 3},
    
    {title: "The clay",
    author: "Tom",
    stars: 2 }

];
// draw shelf
fill(173, 117, 33);
rect(0, 120, width, 10);

// draw one book
for(var i=0; i<book.length; i++){
fill(156, 81, 147);
rect(10 + i*136, 21, 94,100);
fill(0, 0, 0);
text(book[i].title, 15+i*142, 29, 70, 128);
text(book[i].author,15+i*156, 62, 70, 128);
for (var t = 0; t < book[i].stars; t++) {
image(getImage("cute/Star"), 13 + t * 20 + i*146, 90, 20, 30);
}

}
