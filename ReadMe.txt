
Title:		arraylist_examples

Description:	ArrayList SEN article example files
		The article (appearing in Synergy-E-News) presents the use of
		System.Collections.ArrayList as an alternative to using
		%mem_proc and ^m.  The examples (provided here) further
		illustrate the use of both methods.

Author:		John Brunett
		Senior Software Engineer

Date:		8/24/2007

Platforms:	All

Requirements:	Version 9.1.1 and above

Disclaimer:   All code is supplied as seen and without warranty or support,
              and is used at your own risk. Neither the author or Synergex
              accept any responsibility for any loss or damage which may result
              from the use of this code.

===============================================================================

Contents:

		mptest.dbl - example program using %mem_proc and ^m
		altest.dbl - example program using System.Collections.ArrayList
		syntxt.def - include file declaring structures used in 
			     both examples
		arraylist.def - include file defining extended ArrayList class
			     used by altest.dbl

		Files not used in the example (see NOTES):
		Collection.dbl - Workbench template file
		Collection.setemplate - Workbench template file


BUILD instructions:

		dbl mptest
		dblink mptest

		dbl altest
		dblink altest

RUN instructions:

		See comments in either mptest.dbl or altest.dbl

NOTES:		

		The arralist.def include file can be used in any Synergy
		program to generate an ArrayList derived class as-is or
		customized to your needs.

			.define LIST_ITEM, MyStruct
			.define LIST_NAME, MyArrayList
			.include "arraylist.def"

		Replace "MyStruct" with the name of your structure and
		MyArrayList with the name of your ArrayList derived class.

		As an alternative, Workbench users may wish to use the
		provided Workbench templates to generate their own derived
		ArrayList classes (instead of using the arraylist.def file.)

