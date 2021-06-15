.link.current{
    position: relative;
    
}
.link.current::after{
    content: '';
    
    position: absolute;
    bottom: -32px;
    margin-bottom: -1px;

    display: block;
    width: 100%;
    height: 4px;
    background-color: var(--accent-color);
    border: 2px solid;
   
    border-radius: 2px; 
    transition: opacity 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.link.current:hover::after, 
.link.current:focus::after{
    display: block;
    opacity: 1;    
}  