# comp3220-homework-3-solved
**TO GET THIS SOLUTION VISIT:** [COMP3220 Homework 3 Solved](https://www.ankitcodinghub.com/product/comp3220-for-this-assignment-we-will-be-writing-a-parser-that-is-able-to-parse-an-input-file-written-in-our-tiny-grammar-you-should-finish-writing-the-parser-cl/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118107&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP3220 Homework 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
For this assignment, we will be writing a parser that is able to parse an input file written in our “Tiny” grammar. You should finish writing the “Parser” class that I’ve provided. Your Parser class should print:

• Each time it enters or leaves a rule and what the rule is:

Entering [RULE_NAME] Rule

Exiting [RULE_NAME] Rule

There are two exceptions: the ID and the INT rules. In this grammar, ID and INT are also Token names, so we will not print when we are “entering” or “exiting” those rules since we can just check the token type.

• Each time it recognizes a token and what the token was: Found [TOKEN_TYPE] Token: [LEXEME]

For rules with Epsilon definitions, you should also indicate if that definition was chosen:

Did not find [TOKEN_TYPE] or [TOKEN_TYPE] Token, choosing EPSILON production

• Something, everytime it catches an error: Expected [TOKEN_TYPE] found [LEXEME]

When the error could have been multiple things, separate the token types with the word or

Expected [TOKEN_TYPE] or [TOKEN_TYPE] or [TOKEN_TYPE] found [LEXEME]

• How many parse errors were found There were [X] parse errors found.

Parser.rb extends Scanner.rb (The lexer that you wrote for your last assignment) and provides a framework for a topdown, recursive-descent parser of the TINY language. The parser stays one token ahead in the Token stream

(@lookahead) and uses the Token to predict how to continue parsing the current instruction and which method to call next.

The consume() method calls nextToken() in the scanner. The current @lookahead Token is discarded, and the next Token in the stream is retrieved. Whitespace Tokens are discarded.

The match(dtype) method tries to match the @lookahead Token with the provided type (dtype). If a match is found, consume() is called to retrieve the next Token. Otherwise an error message is displayed and then consume() is called to retrieve the next token.

The program() method is first called to parse a TINY program. Since a TINY program consists of a sequence of statements, program() calls statement() repeatedly until it encounters the EOF token.

Complete the parser by providing methods for the appropriate BNF rules in TINY.

I have given you my lexer and token ruby classes. I have also partially written the parser for you and have written a main.rb file that can run your ruby parser. Your assignment is to FINISH WRITING THE PARSER (parser.rb). I have also included 5 sample input files that you can use to test your program once you’ve finished writing it.

input[1-3].txt should complete with no parse errors.

input[4-5].txt should have parse errors.

Below are screenshots of what your output should look like, based on the input files I’ve provided.
