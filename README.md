# Pic-Ception
Going to Disneyland is every child's dream, I too had this dream and I remember the first time I went to Disneyland; the car ride was long and the weather was hot and humid but my seven year old mind knew that this was to be the best trip ever. I remember going on the big roller coasters and thinking I was a big shot when I got to go on a ride my five year old sister was still too small for. One memory that strangely stands out from the rest is eating ice cream in Mickey’s Toontown, it was the biggest ice cream I had ever eaten but that is not why I mention this life changing moment. I was about half way done with my ice cream when I got a brain freeze! I stuck my tongue to the top of my mouth, closed my eyes, and leaned my head back. When I opened my eyes, with my head still back, I saw the most amazing mural in the world; it was a giant mural of Mickey Mouse that covered the entire wall and what made it so special was that within the picture of mickey mouse was thousands of smaller images of all my favorite Disney characters. Since that moment in my childhood I have seen several other photo collages that make up a larger photo but I’ve never come across a program that would create one for you. So this was my purpose, to create a program that would do just that.

## Code Example
'''python
def create(self):
	self._newImage.draw()
	for y in range(0, self._heightB, self._heightS):
		for x in range(0, self._widthB, self._widthS):
			(r, g, b) = self.__getColor(self._bigpic, x, y, self._widthS, self._heightS)
			pic = choice(self._minipics)
			pic = self.__setColor(pic, (r, g, b))
			for yy in range(y, y + self._heightS):
				for xx in range(x, x + self._widthS):
					(r, g, b) = pic.getPixel(xx - x, yy - y)
					self._newImage.setPixel(xx, yy, (r, g, b))
			_root.update()
	#saveAs = filedialog.askdirectory(title = "Save As")
	#saveAs += "/My Picception.gif"
	#self._newImage.save(saveAs)
	_root.mainloop()
'''
## Motivation

My motivation for building this program was primarily for my Python 3 final project, but I was also motivated by the true story I told in the introduction.

## Installation

Download the .zip file "picception.zip". The "main.py" file is where you want to go to run the program.

## Tests

Once you have downloaded the .zip file you will want to open the main.py file and run it, I have provided detailed instructions within the GUI for tests.
