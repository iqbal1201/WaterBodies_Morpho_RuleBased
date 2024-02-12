# WaterBodies_Morpho_RuleBased
Python Function to Classify Water Bodies Based on Rule-Based Decision System

`def class_wb(xclass, yround, zarea):
#cxlass = id represents water bodies or not. class 1 = No, class 2 = water bodies
#yround = roundness. Calculated using formula = (4 * phi * area) / (perimeter * perimeter)
#zarea = if value > 200 hectares or 2000000 meter squares then the class is lake. Otherwise is pond

    if xclass == 2:
    
        if yround > 0.35:
        
            if zarea > 2000000:
            
                return "Lake"
                
            else:
            
                return "Pond"
            
        else:
            return "River"
        
    else:
        return "No"
        `

