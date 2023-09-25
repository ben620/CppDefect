# CppDefect

1. when implement class method, const must be write again, while override/noexcept/explicit does not  
   `  
   //header  
   void React(const EvtSupplyBoxOverlap& e) override const;  
   //body  
   void StNaving::React(const EvtSupplyBoxOverlap& e) const  
   {  
   }  
`   
3. all type declaration is in front of variable name, while array is not    
   `  
   const int *a[];  
   `  
