# WaterBodies_Morpho_RuleBased
Python Function to Classify Water Bodies Based on Rule-Based Decision System


def class_wb(xclass, yround, zarea):
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
