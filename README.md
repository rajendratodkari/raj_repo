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
