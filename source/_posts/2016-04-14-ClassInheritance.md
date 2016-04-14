---
layout: post
title: "Class Inheritance"
date: 2016-04-14 8:40:00
comments: "Class Inheritcance is good"
description: ""
keywords: "Class"
categories:
- Programming
- Class
- OOP
- Ruby
- Comparisons
- Class Inheritance
tags:
- welcome
- done

---


Class inheritance is a very useful tool that coders can use to help with object-oriented programming. Class inheritance allows for the attributes of a “parent” class to be passed on to the subclass of the parent class. Basically, the whole point of class inheritance is to shorten the code that you need to type, thus reducing the small errors that your code sometimes can have. Large companies such as Facebook will use this. Class inheritance is much more useful on a larger scale because there is much more that can be “skipped” when writing the code.

Here is an example from: 

	class Food
		attr_accessor :calorie_content, :fat_content, :amount_of_protein
end

class Meat < Food
	attr_accessor :red, :white

	def red
		redmeat = ["Cow", "Pig", "elk", "Bison"]
		puts redmeat

class Beef < Meat
	attr_accessor :rareness, :chewiness
	def beef_uses
		puts "What is your favorite beef product?"
		beef_preparation = gets.chomp.downcase
		if beef_preparation == "steak"
			puts "nice"
		else
			puts "not nice"
		end
	end


	At the top of the code, the parent class is being created, the Food class. The “attr acessor” the followed by the attributes allows for the coder to not have to type out the reader and writer methods thus further shortening the code. Two or threes lines down I then create the first subclass of the Food class. The notation above is how the subclass receives the attributes of the parent class. In this case my subclass is Meat. Meat is a type of food, not an attribute that a food has, so it works as a perfect subclass.  I then go and define attributes for the Meat class. I see now that red and white meat are types of meats, not a quality of a meat. I should have not had to attributes. Red meat could have been a subclass of Meat and then Beef would have been a subclass of Red Meat. Though, not all things can be inherited from a parent class. Instance variables, for example, can not be inherited through a parent class because instance variables can only be called on in the same block of code. Overall, class inheritance is a very useful tool that can be used to shorten code.
