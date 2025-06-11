**first time**
Jump to: Errors (1) Warnings (1) Validated CSS
W3C CSS Validator results for https://furina662.github.io/92005-Assessment/ (CSS level 3 + SVG)

Sorry! We found the following errors (1)
URI : https://furina662.github.io/92005-Assessment/css/index.css
line98	
.main-content	Parse Error container { margin: 0; padding: 50px 30px; width: 90%; max-width: none; } 
.container h1 { font-size: 3rem; } 
.intro-text { font-size: 1.2rem; padding: 25px; }

Warnings (1)
URI : https://furina662.github.io/92005-Assessment/css/index.css
line84		
container is a CSS hack



**original code**
@media (max-width: 768px) {
    .main-content {
        min-height: calc(100vh - 100px); 
        padding-top: 40px;
           
    
    .container {
        margin: 0;                  
        padding: 50px 30px;          
        width: 90%;                 
        max-width: none;   
    }
    
    .container h1 {
        font-size: 3rem;              
    }
    
    .intro-text {
        font-size: 1.2rem;            
        padding: 25px;              
    }
}



**fixed code:**
@media (max-width: 768px) {
    .main-content {
        min-height: calc(100vh - 100px); 
        padding-top: 40px;
           
    }
    .container {
        margin: 0;                  
        padding: 50px 30px;          
        width: 90%;                 
        max-width: none;   
    }
    
    .container h1 {
        font-size: 3rem;              
    }
    
    .intro-text {
        font-size: 1.2rem;            
        padding: 25px;              
    }
}

**Reason: main-content is missing a closing bracket**