# drainage
Application to calculate and publish civil engineering site drainage calcualtions

Currently generating project requirements

## Glossary
IAW - shorthand for 'in accordance with'

basin - Area of land where all precipitation that falls will drain or flow downhill to a specific collection point.  The collection point can be a street drain, stream, or other structure.

IDF - Intensity, duration, frequency curves describing rainfall in a given area.

T<sub>c</sub> - Time of conentration.  How long does it take for rainfall within a drainage basin to travel from the farthest point to the collection point. Usually calculated using the TR-55 method as described by the USDA/NRCS

overland flow - Flow of rainfall run-off over open land.  Not contained in a gutter, pipe, or other conveyance system.

gutter flow - Flow of rainfall within street gutters.

pipe flow - Flow of rainfall through gravity driven storm drain pipes.  No pressurized or fully flowing pipes.

## Requirements
1. Resulting report must be publishable as a pdf document.
2. Must not use a single 'master' database, but use project level databases.  While this application may be open-source, the data and the results are proprietary and may not be mingled between projects or clients.
3. Report format is as follows
  * Cover page
  
    Include project name, number, municipality, county/state, publish date (month/year), corporate logo and address.
    Also, include space to accomodate either an engineer's (P.E.) wet stamp and signature or a digital copy as allowed by state law.
  
  * Narrative
  
    Include at least these editable sections: Site Overview, Existing Site Characteristics, Drainage Design Concept, Calculation Methods, Soil Conditions.  Additional sections can be added as desired.
    
  * Calculations
  
    Separate page(s) for each drainage basin 
  
  * Supporting documents
  
    IDF (rainfall Intensity/Duration/Frequency) curve with data table for each IDF curve used.  Most projects use only one, but anticipate the need to use multiple IDF curves on a project.
    
4. Calculations 
  * Allow each basin to contain multiple sub-basins.
  * Perform T<sub>c</sub> calculations IAW TR-55 for both overland flow and gutter flow
  * Allow the user to enter a fixed runoff coefficient value or calculate a composite runoff coefficient value
