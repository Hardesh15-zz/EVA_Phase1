## Asignment 1B
### 1. What are Channels and Kernels (according to EVA)?
* Channels are collection of similer features of objects/texts/colors/etc. Examples- 1) Collection of all blue colors is blue channel 2) collection of all 'H' texts is also a channel.
* Kernel is a filter/feature extractor/3x3. it applies on input image to get output though convolution layers. Example- When we apply 3x3 filter over image of 7X7 we get output image of 5x5 through convolution operation.
### 2. Why should we only (well mostly) use 3x3 Kernels?
1. we will get lower number of weights. it means that it's computational efficiency will be high.
2. we will get more number of layers which captures complex features as well.
3. Odd size filters are prefered because they capture distortions across the layers which is not possible in even size filter due to symmetry.
### 3. How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)
**99 times** 
* 199|197|195|193|191|--> 5 convolution operation
* 189|187|185|183|181|--> 5 convolution operation
* 179|177|175|173|171|--> 5 convolution operation
* 169|167|165|163|161|--> 5 convolution operation
* 159|157|155|153|151|--> 5 convolution operation
* 149|147|145|143|141|--> 5 convolution operation
* 139|137|135|133|131|--> 5 convolution operation
* 129|127|125|123|121|--> 5 convolution operation
* 119|117|115|113|111|--> 5 convolution operation
* 109|107|105|103|101|--> 5 convolution operation
* 99|97|95|93|91|     --> 5 convolution operation
* 89|87|85|83|81|     --> 5 convolution operation
* 79|77|75|73|71|     --> 5 convolution operation
* 69|67|65|63|61|     --> 5 convolution operation
* 59|57|55|53|51|     --> 5 convolution operation
* 49|47|45|43|41|     --> 5 convolution operation
* 39|37|35|33|31|     --> 5 convolution operation
* 29|27|25|23|21|     --> 5 convolution operation
* 19|17|15|13|11|     --> 5 convolution operation
* 9|7|5|3|1x1         --> 4 convolution operation  
*Total Number of convolution operation = 5x19+4 = 99*
