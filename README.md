# Vim Plugins & their usages

## 1. tpope/vim-commentary

    **Normal Mode**
    
      gcc OR 5gcc - 
        comment out number of lines
        
      gc - 
        comment out target of motion
          like  gcap - comment out paragraph
                gci{ - comment out all line in {}
                gcaw - comment out all line including {}
        comment out in visual mode
        
     **Command Mode**
     
      :7,17Commentary -
        comment out range of lines
        
      :g/keyword/Commentary -
        comment out all lines containing string 'keyword'
        
## 2. tpope/vim-surround

	**Normal Mode**
	
	Hello World!		csw"			"Hello" World!		--	single	world (w)
	Hello World!		css"			"Hello World!"		--	whole sentence (s)
	"Hello World!"		cs"'			'Hello World!'
	"Hello World!"		cd"<q>			<q>Hello World</q>
	<q>Hello World</q>	cst'			'Hello World'
	"Hello World!"		ds"			Hello World!
	Hello World		ysiw[ OR ysaw[		[ Hello ] World!		--	cursor on Hello
	Hello World		ysiw] OR ysaw]		[Hello] World!			--	cursor on Hello
	[Hello] World		yss) OR yssb		([Hello] World!)
	([Hello] World!)	ds[ds(			Hello World!			--	remove specific surrounding
	Hello World!		ysiw<p>			<p>Hello</p> World!
	
	**Visual Line Mode**
	<p>Hello</p> World!	S<div class="temp">(hit return)		<div class"temp">
										<p>Hello</p> World!
									</div>
	
## 3. tpope/vim-ragtag

	**Insert Mode**
	
	CTRL+X !		new Doctype Declartion
	CTRL+X @		new css tag
	CTRL+X #		new meta tag
	CTRL+X $		new javascript tag
	
	Mapping    Result
	---------  -----------
	CTRL+X =   foo<%= | %>
	CTRL+X +   <%= foo| %>
	CTRL+X -   foo<% | %>
	CTRL+X _   <% foo| %>
	CTRL+X '   foo<%# | %>
	CTRL+X "   <%# foo| %>
	
	
