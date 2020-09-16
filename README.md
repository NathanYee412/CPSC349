"# CPSC349" 
Ottergram front end web development project 
Nathan Yee
Resources from BNR 



 


#############################################################################
NOTES

 (In general, the order of your
styles only matters when you have multiple rule sets for the same selector. In Ottergram, the styles are
arranged in roughly the same order as they appear in the code. This is a matter of preference, and you
are free to organize your styles as you see fit.)

.thumbnail-item {
 background: blue;
 }
li {
 background: red;
}

Both of these match your <li> elements. What background color will your <li> elements have?
Even though the li { background: red; } rule is more recent, .thumbnail-item { background:
blue; } will be used. Why? Because it uses a class selector, which is more specific (i.e., assigned a
higher specificity value) than the element selector.



https://specificity.keegan.st/
used to calculate specificity 



flex: 0 1 auto;
0: flex-grow
1: flex-shrink
auto: flex-basis 

0 1 auto = i do not want to grow any larger; I will shrink as needed; please calculate my size for me;

flex-grow: 1 = i would like to grow as much as possible 



#############################################################################




#############################################################################
html changes 

            <a href="img/otter1.jpg" data-image-role="trigger" 
                                     data-image-title="Stayin' Alive"
                                     data-image-url="img/otter1.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/otter1.jpg" alt="Barry the Otter">
                    <span class="thumbnail-title">Barry</span>
                </li>
            </a>

changed to 

            <li class="thumbnail-item>
                <a href="img/otter1.jpg" data-image-role="trigger" 
                                         data-image-title="Stayin' Alive"
                                         data-image-url="img/otter1.jpg">
                    <img class="thumbnail-image" src="img/otter1.jpg alt="Barry the Otter">
                    <span class="thumbnail-title">Barry</span>
                </a>
            </li>





#############################################################################
backup of original html structure 

           <a href="img/otter2.jpg" data-image-role="trigger" data-image-title="How Deep is Your Love?"
                data-image-url="img/otter2.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/otter2.jpg" alt="Robin the Otter">
                    <span class="thumbnail-title">Robin</span>
                </li>
            </a>
            <a href="img/otter3.jpg" data-image-role="trigger" data-image-title="You Should Be Dancing"
                data-image-url="img/otter3.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/otter3.jpg" alt="Maurice the Otter">
                    <span class="thumbnail-title">Maurice</span>
                </li>
            </a>
            <a href="img/otter4.jpg" data-image-role="trigger" data-image-title="Stayin' Alive"
                data-image-url="img/otter4.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/otter4.jpg" alt="Lesley the Otter">
                    <span class="thumbnail-title">Lesley</span>
                </li>
            </a>
            <a href="img/otter5.jpg" data-image-role="trigger" data-image-title="Stayin' Alive"
                data-image-url="img/otter5.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/otter5.jpg" alt="Barbara the Otter">
                    <span class="thumbnail-title">Barbara</span>
                </li>
            </a>
            <a href="img/gridGarden.png" data-image-role="trigger" data-image-title="Stayin' Alive"
                data-image-url="img/gridGarden.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/gridGarden.png" alt="Grid Garden">
                    <span class="thumbnail-title">Grid Garden</span>
                </li>
            </a>
            <a href="img/flexboxFroggy.png" data-image-role="trigger" data-image-title="Stayin' Alive"
                data-image-url="img/flexboxFroggy.jpg">
                <li class="thumbnail-item">
                    <img class="thumbnail-image" src="img/flexboxFroggy.png" alt="Flexbox Froggy">
                    <span class="thumbnail-title">Flexbox Froggy</span>
                </li>
            </a>
