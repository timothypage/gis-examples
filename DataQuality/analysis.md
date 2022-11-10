xpath -e '//mdq:DQ_DataQuality'
xpath -e '//dataqual' 

[USGS_US_Topo_Map_Collection.xml](https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/USGS_US_Topo_Map_Collection.xml)

works

fgdc
```xml
<dataqual>
    <attracc>
      <attraccr>Cartographic content is derived from USGS national geospatial databases. The data is
        owned and hosted by the USGS, but does not preclude using data sources owned and hosted by
        other organizations, provided that these sources have been approved by the USGS data
        program.</attraccr>
    </attracc>
    <logic>This product is a layered geospatial PDF file.</logic>
    <complete>Each PDF layer is derived from data extracted from USGS national geospatial databases. These data are intended to be cartographically complete at 1:24,000 scale.</complete>
    <posacc>
      <horizpa>
        <horizpar>This US Topo map product is compiled to meet National Map Accuracy Standards
          (NMAS). NMAS horizontal accuracy requires that at least 90 percent of well-defined points
          tested are within 0.02 inch of the true position. In this product, the projection line,
          grids, and orthoimage are believed to meet NMAS. Positional accuracy of the other data
          layers is less controllable because of diversity of data sources, and may not meet
          NMAS.</horizpar>
      </horizpa>
      <vertacc>
        <vertaccr>US Topo contours are derived from the USGS 3D Elevation Program (3DEP) 1/3 arc-second DEM data. Accuracy of 3DEP is inherited from various sources. These data sources vary in vertical accuracy depending on time of collection, collection method, control accuracy and density, and local terrain relief. The overall absolute vertical accuracy of the 1/3 arcsecond DEM data, as tested against GPS control, is about 3 meters at 95% confidence level (National Standards for Spatial Data Accuracy). US Topo contours are derived from the DEMs to generally meet National Map Accuracy Standards (90% of well-defined points in reasonably level terrain test within one-half contour interval of the true ground elevation); however, actual vertical accuracies of individual US Topo quadrangles may not meet that standard. Quadrangles containing collar notes stating contours "May not meet National Map Accuracy Standards" are in areas where the source is known to be questionable for meeting NMAS for the stated contour interval.</vertaccr>
      </vertacc>
    </posacc>
    <lineage>
      <procstep>
        <procdesc>The geospatial PDFs for this product are created as follows. All geospatial content is
          taken from national geospatial databases under the stewardship of USGS data programs. The
          NAIP imagery is provided by a seamless tile service that delivers image data at the
          resolution and quality of the source imagery. The raster and vector data, including grids
          and collar information, are processed using ESRI ArcGIS software and exported as a geospatial PDF.
          application, which includes post-processing to embed the metadata XML document.
          Any use of trade, product, or firm names in this publication is for descriptive purposes
          only and does not imply endorsement by the U.S. Government.</procdesc>
        <procdate>2022</procdate>
      </procstep>
    </lineage>
  </dataqual>
```

mdTranslator iso
```xml
<mdq:DQ_DataQuality>
   <mdq:scope>
      <mcc:MD_Scope>
         <mcc:level>
            <mcc:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeListValue="series" />
         </mcc:level>
      </mcc:MD_Scope>
   </mdq:scope>
   <mdq:report>
      <mdq:DQ_NonQuantitativeAttributeCompleteness>
         <mdq:result>
            <mdq:DQ_DescriptiveResult>
               <mdq:statement>
                  <gco:CharacterString>Cartographic content is derived from USGS national geospatial databases. The data is
  owned and hosted by the USGS, but does not preclude using data sources owned and hosted by
  other organizations, provided that these sources have been approved by the USGS data
  program.</gco:CharacterString>
               </mdq:statement>
            </mdq:DQ_DescriptiveResult>
         </mdq:result>
      </mdq:DQ_NonQuantitativeAttributeCompleteness>
   </mdq:report>
   <mdq:report>
      <mdq:DQ_ConceptualConsistency>
         <mdq:measure>
            <mdq:DQ_MeasureReference>
               <mdq:measureDescription>
                  <gco:CharacterString>This product is a layered geospatial PDF file.</gco:CharacterString>
               </mdq:measureDescription>
            </mdq:DQ_MeasureReference>
         </mdq:measure>
      </mdq:DQ_ConceptualConsistency>
   </mdq:report>
   <mdq:report>
      <mdq:DQ_CompletenessOmission>
         <mdq:result>
            <mdq:DQ_DescriptiveResult>
               <mdq:statement>
                  <gco:CharacterString>Each PDF layer is derived from data extracted from USGS national geospatial databases. These data are intended to be cartographically complete at 1:24,000 scale.</gco:CharacterString>
               </mdq:statement>
            </mdq:DQ_DescriptiveResult>
         </mdq:result>
      </mdq:DQ_CompletenessOmission>
   </mdq:report>
   <mdq:report>
      <mdq:DQ_CompletenessCommission>
         <mdq:result>
            <mdq:DQ_DescriptiveResult>
               <mdq:statement>
                  <gco:CharacterString>Each PDF layer is derived from data extracted from USGS national geospatial databases. These data are intended to be cartographically complete at 1:24,000 scale.</gco:CharacterString>
               </mdq:statement>
            </mdq:DQ_DescriptiveResult>
         </mdq:result>
      </mdq:DQ_CompletenessCommission>
   </mdq:report>
   <mdq:report>
      <mdq:DQ_AbsoluteExternalPositionalAccuracy>
         <mdq:evaluationMethod>
            <mdq:DQ_EvaluationMethod>
               <mdq:evaluationMethodDescription>
                  <gco:CharacterString>This US Topo map product is compiled to meet National Map Accuracy Standards
    (NMAS). NMAS horizontal accuracy requires that at least 90 percent of well-defined points
    tested are within 0.02 inch of the true position. In this product, the projection line,
    grids, and orthoimage are believed to meet NMAS. Positional accuracy of the other data
    layers is less controllable because of diversity of data sources, and may not meet
    NMAS.</gco:CharacterString>
               </mdq:evaluationMethodDescription>
            </mdq:DQ_EvaluationMethod>
         </mdq:evaluationMethod>
         <mdq:measure>
            <mdq:DQ_MeasureReference>
               <mdq:nameOfMeasure>
                  <gco:CharacterString>Horizontal Positional Accuracy Report</gco:CharacterString>
               </mdq:nameOfMeasure>
            </mdq:DQ_MeasureReference>
         </mdq:measure>
      </mdq:DQ_AbsoluteExternalPositionalAccuracy>
   </mdq:report>
   <mdq:report>
      <mdq:DQ_AbsoluteExternalPositionalAccuracy>
         <mdq:evaluationMethod>
            <mdq:DQ_EvaluationMethod>
               <mdq:evaluationMethodDescription>
                  <gco:CharacterString>US Topo contours are derived from the USGS 3D Elevation Program (3DEP) 1/3 arc-second DEM data. Accuracy of 3DEP is inherited from various sources. These data sources vary in vertical accuracy depending on time of collection, collection method, control accuracy and density, and local terrain relief. The overall absolute vertical accuracy of the 1/3 arcsecond DEM data, as tested against GPS control, is about 3 meters at 95% confidence level (National Standards for Spatial Data Accuracy). US Topo contours are derived from the DEMs to generally meet National Map Accuracy Standards (90% of well-defined points in reasonably level terrain test within one-half contour interval of the true ground elevation); however, actual vertical accuracies of individual US Topo quadrangles may not meet that standard. Quadrangles containing collar notes stating contours "May not meet National Map Accuracy Standards" are in areas where the source is known to be questionable for meeting NMAS for the stated contour interval.</gco:CharacterString>
               </mdq:evaluationMethodDescription>
            </mdq:DQ_EvaluationMethod>
         </mdq:evaluationMethod>
         <mdq:measure>
            <mdq:DQ_MeasureReference>
               <mdq:nameOfMeasure>
                  <gco:CharacterString>Vertical Positional Accuracy Report</gco:CharacterString>
               </mdq:nameOfMeasure>
            </mdq:DQ_MeasureReference>
         </mdq:measure>
      </mdq:DQ_AbsoluteExternalPositionalAccuracy>
   </mdq:report>
</mdq:DQ_DataQuality>
```


https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/USGS_3DEP_DEM_Source_OPR_Collection.xml

works

fgdc
```xml
<dataqual>
  <logic>Please refer to the copy of the original product metadata file within the delivered folder if one was provided.</logic>
  <complete>Data set is considered complete for the information presented, as described in the abstract. Users are advised to read the rest of the metadata record carefully for additional details.</complete>
  <posacc>
    <vertacc>
    <vertaccr>Please refer to the copy of the original product metadata file if one was provided.</vertaccr>
    </vertacc>
  </posacc>
  <lineage>
    <procstep>
      <procdesc>Original project data were provided to the National Geospatial Technical Operations Center (NGTOC) in Rolla, MO and/or Denver, CO. The data were reviewed for quality and accuracy before publication. Data are provided in the original source resolution and spatial reference.</procdesc>
      <procdate>2022</procdate>
    </procstep>
  </lineage>
</dataqual>
```

mdTranslator iso
```xml
<mdq:DQ_DataQuality>
  <mdq:scope>
    <mcc:MD_Scope>
       <mcc:level>
          <mcc:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeListValue="series" />
       </mcc:level>
    </mcc:MD_Scope>
  </mdq:scope>
  <mdq:report>
    <mdq:DQ_NonQuantitativeAttributeCompleteness>
       <mdq:result>
          <mdq:DQ_DescriptiveResult>
          </mdq:DQ_DescriptiveResult>
       </mdq:result>
    </mdq:DQ_NonQuantitativeAttributeCompleteness>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_ConceptualConsistency>
       <mdq:measure>
          <mdq:DQ_MeasureReference>
             <mdq:measureDescription>
                <gco:CharacterString>Please refer to the copy of the original product metadata file within the delivered folder if one was provided.</gco:CharacterString>
             </mdq:measureDescription>
          </mdq:DQ_MeasureReference>
       </mdq:measure>
    </mdq:DQ_ConceptualConsistency>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessOmission>
       <mdq:result>
          <mdq:DQ_DescriptiveResult>
             <mdq:statement>
                <gco:CharacterString>Data set is considered complete for the information presented, as described in the abstract. Users are advised to read the rest of the metadata record carefully for additional details.</gco:CharacterString>
             </mdq:statement>
          </mdq:DQ_DescriptiveResult>
       </mdq:result>
    </mdq:DQ_CompletenessOmission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessCommission>
       <mdq:result>
          <mdq:DQ_DescriptiveResult>
             <mdq:statement>
                <gco:CharacterString>Data set is considered complete for the information presented, as described in the abstract. Users are advised to read the rest of the metadata record carefully for additional details.</gco:CharacterString>
             </mdq:statement>
          </mdq:DQ_DescriptiveResult>
       </mdq:result>
    </mdq:DQ_CompletenessCommission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_AbsoluteExternalPositionalAccuracy>
       <mdq:evaluationMethod>
          <mdq:DQ_EvaluationMethod>
             <mdq:evaluationMethodDescription>
                <gco:CharacterString>Please refer to the copy of the original product metadata file if one was provided.</gco:CharacterString>
             </mdq:evaluationMethodDescription>
          </mdq:DQ_EvaluationMethod>
       </mdq:evaluationMethod>
       <mdq:measure>
          <mdq:DQ_MeasureReference>
             <mdq:nameOfMeasure>
                <gco:CharacterString>Vertical Positional Accuracy Report</gco:CharacterString>
             </mdq:nameOfMeasure>
          </mdq:DQ_MeasureReference>
       </mdq:measure>
    </mdq:DQ_AbsoluteExternalPositionalAccuracy>
  </mdq:report>
</mdq:DQ_DataQuality>
```

https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/USGS_3DEP_LidarPointCloud_Collection-csdgm.xml

works

fgdc
```xml
<dataqual>
  <attracc>
    <attraccr>Data are provided in las format version LAZ 1.4. Header attributes and point attribute for LAS files can be found on ASPRS website listed below. USGS not making any promises on the accuracy or completeness of the attribute information.</attraccr>
  </attracc>
  <logic>Please refer to the Metadata Section at the end of this document for a live link to a copy of the original data source's metadata file if one was provided.</logic>
  <complete>The lidar collection has been acquired by the USGS through contracts, partnerships with other Federal, state, tribal, or regional agencies, from direct purchases from private industry vendors, and through volunteer contributions from the science community. While USGS makes every effort to provide accurate and complete information, USGS provides no warranty, expressed or implied, as to the accuracy, reliability or completeness of furnished lidar point clouds. Please note that USGS does not control and cannot guarantee the relevance, timeliness, or accuracy of these outside materials.</complete>
  <lineage>
    <procstep>
      <procdesc>unknown</procdesc>
      <procdate>2022</procdate>
    </procstep>
  </lineage>
</dataqual>
```

mdTranslator iso
```xml
<mdq:DQ_DataQuality>
  <mdq:scope>
    <mcc:MD_Scope>
      <mcc:level>
        <mcc:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeListValue="series"/>
      </mcc:level>
    </mcc:MD_Scope>
  </mdq:scope>
  <mdq:report>
    <mdq:DQ_NonQuantitativeAttributeCompleteness>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
                  </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_NonQuantitativeAttributeCompleteness>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_ConceptualConsistency>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:measureDescription>
            <gco:CharacterString>Please refer to the copy of the original product metadata file within the delivered folder if one was provided.</gco:CharacterString>
          </mdq:measureDescription>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_ConceptualConsistency>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessOmission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>Data set is considered complete for the information presented, as described in the abstract. Users are advised to read the rest of the metadata record carefully for additional details.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessOmission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessCommission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>Data set is considered complete for the information presented, as described in the abstract. Users are advised to read the rest of the metadata record carefully for additional details.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessCommission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_AbsoluteExternalPositionalAccuracy>
      <mdq:evaluationMethod>
        <mdq:DQ_EvaluationMethod>
          <mdq:evaluationMethodDescription>
            <gco:CharacterString>Please refer to the copy of the original product metadata file if one was provided.</gco:CharacterString>
          </mdq:evaluationMethodDescription>
        </mdq:DQ_EvaluationMethod>
      </mdq:evaluationMethod>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:nameOfMeasure>
            <gco:CharacterString>Vertical Positional Accuracy Report</gco:CharacterString>
          </mdq:nameOfMeasure>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_AbsoluteExternalPositionalAccuracy>
  </mdq:report>
</mdq:DQ_DataQuality>
```



https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/National_Wetlands_Inventory_Wetlands-csdgm.xml

  Message: 1
  ERROR: ISO-19115-1 writer: spatial reference system identifier is missing: CONTEXT is resource spatial reference system

  Message: 2
  ERROR: ISO-19115-1 writer: spatial reference system type is missing: CONTEXT is resource spatial reference system

  Message: 3
  ERROR: ISO-19115-1 writer: spatial reference system identifier is missing: CONTEXT is resource spatial reference system

  Message: 4
  ERROR: ISO-19115-1 writer: spatial reference system type is missing: CONTEXT is resource spatial reference system

  -f=false works though

fgdc

    xpath -n -e '//dataqual' ~/geoplatform/gis-examples/DataQuality/xml/National_Wetlands_Inventory_Wetlands-csdgm.xml | xmllint --format - | tail -n +2 | pbcopy

```xml
<dataqual>
  <attracc>
    <attraccr>Data accuracy is ensured using standard review procedures including visual inspection as well as automated verification routines.  Automated verification is designed to address specific geospatial errors, digital anomalies and logic checks.  Quality of the attribute information varies with age and mapping protocols used when individual maps were prepared.</attraccr>
    <qattracc>
      <attraccv>100%</attraccv>
      <attracce>All polygons are attributed.</attracce>
    </qattracc>
  </attracc>
  <logic>Polygon and chain-node topology are present. Every polygon has a label.</logic>
  <complete>This data set represents the extent of wetlands and deepwater habitats that can be determined with the use of remotely sensed data and within the time frame for which the maps were produced. Wetlands are shown in all of the 50 states, the District of Columbia, Puerto Rico, the Virgin Islands, Guam and Saipan.  The accuracy of image interpretation depends on the quality of the imagery, the experience of the image analysts, the amount and quality of the collateral data, and the amount of ground truth verification work conducted.  

There is a margin error inherent in the use of imagery, thus detailed on-the-ground inspection of any particular site, may result in revision of the wetland boundaries or classification, established through image analysis.

Wetlands or other mapped features may have changed since the date or the imagery and/or field work.  There may be occasional differences in polygon boundaries or classifications between the information depicted on the map and the actual conditions on site.</complete>
  <lineage>
  ...
  </lineage>
</dataqual>
```

mdTranslator iso
    
    bundle exec ./bin/mdtranslator translate --reader=fgdc --writer=iso19115_1 ~/geoplatform/gis-examples/DataQuality/xml/National_Wetlands_Inventory_Wetlands-csdgm.xml | xpath -e '//mdq:DQ_DataQuality' | xmllint --format - | tail -n +2

```xml
<mdq:DQ_DataQuality>
  <mdq:scope>
    <mcc:MD_Scope>
      <mcc:level>
        <mcc:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeListValue="series"/>
      </mcc:level>
    </mcc:MD_Scope>
  </mdq:scope>
  <mdq:report>
    <mdq:DQ_NonQuantitativeAttributeCompleteness>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>Data accuracy is ensured using standard review procedures including visual inspection as well as automated verification routines.  Automated verification is designed to address specific geospatial errors, digital anomalies and logic checks.  Quality of the attribute information varies with age and mapping protocols used when individual maps were prepared.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_NonQuantitativeAttributeCompleteness>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_ConceptualConsistency>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:measureDescription>
            <gco:CharacterString>Polygon and chain-node topology are present. Every polygon has a label.</gco:CharacterString>
          </mdq:measureDescription>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_ConceptualConsistency>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessOmission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>This data set represents the extent of wetlands and deepwater habitats that can be determined with the use of remotely sensed data and within the time frame for which the maps were produced. Wetlands are shown in all of the 50 states, the District of Columbia, Puerto Rico, the Virgin Islands, Guam and Saipan.  The accuracy of image interpretation depends on the quality of the imagery, the experience of the image analysts, the amount and quality of the collateral data, and the amount of ground truth verification work conducted.  

There is a margin error inherent in the use of imagery, thus detailed on-the-ground inspection of any particular site, may result in revision of the wetland boundaries or classification, established through image analysis.

Wetlands or other mapped features may have changed since the date or the imagery and/or field work.  There may be occasional differences in polygon boundaries or classifications between the information depicted on the map and the actual conditions on site.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessOmission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessCommission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>This data set represents the extent of wetlands and deepwater habitats that can be determined with the use of remotely sensed data and within the time frame for which the maps were produced. Wetlands are shown in all of the 50 states, the District of Columbia, Puerto Rico, the Virgin Islands, Guam and Saipan.  The accuracy of image interpretation depends on the quality of the imagery, the experience of the image analysts, the amount and quality of the collateral data, and the amount of ground truth verification work conducted.  

There is a margin error inherent in the use of imagery, thus detailed on-the-ground inspection of any particular site, may result in revision of the wetland boundaries or classification, established through image analysis.

Wetlands or other mapped features may have changed since the date or the imagery and/or field work.  There may be occasional differences in polygon boundaries or classifications between the information depicted on the map and the actual conditions on site.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessCommission>
  </mdq:report>
</mdq:DQ_DataQuality>
```


https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/USGS_NHD_Collection.xml


  Message: 1
  ERROR: ISO-19115-1 writer: spatial reference system identifier is missing: CONTEXT is resource spatial reference system

  Message: 2
  ERROR: ISO-19115-1 writer: spatial reference system type is missing: CONTEXT is resource spatial reference system

  -f=false works though

    xpath -n -e '//dataqual' ~/geoplatform/gis-examples/DataQuality/xml/USGS_NHD_Collection.xml | xmllint --format - | tail -n +2 | pbcopy

fgdc
```xml
<dataqual>
  <attracc>
    <attraccr>Statements of attribute accuracy are based on accuracy statements made for U.S. Geological Survey Digital Line Graph (DLG) data, which is estimated to be 98.5 percent. One or more of the following methods were used to test attribute accuracy: manual comparison of the source with hardcopy plots; symbolized display of the DLG on an interactive computer graphic system; selected attributes that could not be visually verified on plots or on screen were interactively queried and verified on screen. In addition, software validated feature types and characteristics against a master set of types and characteristics, checked that combinations of types and characteristics were valid, and that types and characteristics were valid for the delineation of the feature. Feature types, characteristics, and other attributes conform to the Standards for National Hydrography Dataset (USGS, 1999) as of the date they were loaded into the database. All names were validated against a current extract from the Geographic Names Information System (GNIS). The entry and identifier for the names match those in the GNIS. The association of each name to reaches has been interactively checked, however, operator error could in some cases apply a name to a wrong reach.</attraccr>
  </attracc>
  <logic>Points, nodes, lines, and areas conform to topological rules. Lines intersect only at nodes, and all nodes anchor the ends of lines. Lines do not overshoot or undershoot other lines where they are supposed to meet. There are no duplicate lines. Lines bound areas and lines identify the areas to the left and right of the lines. Gaps and overlaps among areas do not exist. All areas close.</logic>
  <complete> The completeness of the data reflects the content of the sources, which most often are the published USGS topographic quadrangle and/or the USDA Forest Service Primary Base Series (PBS) map. The USGS topographic quadrangle is usually supplemented by Digital Orthophoto Quadrangles (DOQs). Features found on the ground may have been eliminated or generalized on the source map because of scale and legibility constraints. In general, streams longer than one mile (approximately 1.6 kilometers) were collected. Most streams that flow from a lake were collected regardless of their length. Only definite channels were collected so not all swamp/marsh features have stream/rivers delineated through them. Lake/ponds having an area greater than 6 acres were collected. Note, however, that these general rules were applied unevenly among maps during compilation. Reach codes are defined on all features of type stream/river, canal/ditch, artificial path, coastline, and connector. Waterbody reach codes are defined on all lake/pond and most reservoir features. Names were applied from the GNIS database. Detailed capture conditions are provided for every feature type in the Standards for National Hydrography Dataset available online through https://prd-wret.s3-us-west-2.amazonaws.com/assets/palladium/production/atoms/files/NHD%201999%20Draft%20Standards%20-%20Capture%20conditions.PDF.</complete>
  <posacc>
    <horizpa>
      <horizpar>Statements of horizontal positional accuracy are based on accuracy statements made for U.S. Geological Survey topographic quadrangle maps. These maps were compiled to meet National Map Accuracy Standards. For horizontal accuracy, this standard is met if at least 90 percent of points tested are within 0.02 inch (at map scale) of the true position. Additional offsets to positions may have been introduced where feature density is high to improve the legibility of map symbols. In addition, the digitizing of maps is estimated to contain a horizontal positional error of less than or equal to 0.003 inch standard error (at map scale) in the two component directions relative to the source maps. Visual comparison between the map graphic (including digital scans of the graphic) and plots or digital displays of points, lines, and areas, is used as control to assess the positional accuracy of digital data. Digital map elements along the adjoining edges of data sets are aligned if they are within a 0.02 inch tolerance (at map scale). Features with like dimensionality (for example, features that all are delineated with lines), with or without like characteristics, that are within the tolerance are aligned by moving the features equally to a common point. Features outside the tolerance are not moved; instead, a feature of type connector is added to join the features.</horizpar>
    </horizpa>
    <vertacc>
      <vertaccr>Statements of vertical positional accuracy for elevation of water surfaces are based on accuracy statements made for U.S. Geological Survey topographic quadrangle maps. These maps were compiled to meet National Map Accuracy Standards. For vertical accuracy, this standard is met if at least 90 percent of well-defined points tested are within one-half contour interval of the correct value. Elevations of water surface printed on the published map meet this standard; the contour intervals of the maps vary. These elevations were transcribed into the digital data; the accuracy of this transcription was checked by visual comparison between the data and the map.</vertaccr>
    </vertacc>
  </posacc>
  <lineage>
  ...
  </lineage>
</dataqual>
```

    bundle exec ./bin/mdtranslator translate -f=false --reader=fgdc --writer=iso19115_1 ~/geoplatform/gis-examples/DataQuality/xml/USGS_NHD_Collection.xml | xpath -e '//mdq:DQ_DataQuality' | xmllint --format - | tail -n +2

mdTranslator iso
```xml
<mdq:DQ_DataQuality>
  <mdq:scope>
    <mcc:MD_Scope>
      <mcc:level>
        <mcc:MD_ScopeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_ScopeCode" codeListValue="series"/>
      </mcc:level>
    </mcc:MD_Scope>
  </mdq:scope>
  <mdq:report>
    <mdq:DQ_NonQuantitativeAttributeCompleteness>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString>Statements of attribute accuracy are based on accuracy statements made for U.S. Geological Survey Digital Line Graph (DLG) data, which is estimated to be 98.5 percent. One or more of the following methods were used to test attribute accuracy: manual comparison of the source with hardcopy plots; symbolized display of the DLG on an interactive computer graphic system; selected attributes that could not be visually verified on plots or on screen were interactively queried and verified on screen. In addition, software validated feature types and characteristics against a master set of types and characteristics, checked that combinations of types and characteristics were valid, and that types and characteristics were valid for the delineation of the feature. Feature types, characteristics, and other attributes conform to the Standards for National Hydrography Dataset (USGS, 1999) as of the date they were loaded into the database. All names were validated against a current extract from the Geographic Names Information System (GNIS). The entry and identifier for the names match those in the GNIS. The association of each name to reaches has been interactively checked, however, operator error could in some cases apply a name to a wrong reach.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_NonQuantitativeAttributeCompleteness>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_ConceptualConsistency>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:measureDescription>
            <gco:CharacterString>Points, nodes, lines, and areas conform to topological rules. Lines intersect only at nodes, and all nodes anchor the ends of lines. Lines do not overshoot or undershoot other lines where they are supposed to meet. There are no duplicate lines. Lines bound areas and lines identify the areas to the left and right of the lines. Gaps and overlaps among areas do not exist. All areas close.</gco:CharacterString>
          </mdq:measureDescription>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_ConceptualConsistency>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessOmission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString> The completeness of the data reflects the content of the sources, which most often are the published USGS topographic quadrangle and/or the USDA Forest Service Primary Base Series (PBS) map. The USGS topographic quadrangle is usually supplemented by Digital Orthophoto Quadrangles (DOQs). Features found on the ground may have been eliminated or generalized on the source map because of scale and legibility constraints. In general, streams longer than one mile (approximately 1.6 kilometers) were collected. Most streams that flow from a lake were collected regardless of their length. Only definite channels were collected so not all swamp/marsh features have stream/rivers delineated through them. Lake/ponds having an area greater than 6 acres were collected. Note, however, that these general rules were applied unevenly among maps during compilation. Reach codes are defined on all features of type stream/river, canal/ditch, artificial path, coastline, and connector. Waterbody reach codes are defined on all lake/pond and most reservoir features. Names were applied from the GNIS database. Detailed capture conditions are provided for every feature type in the Standards for National Hydrography Dataset available online through https://prd-wret.s3-us-west-2.amazonaws.com/assets/palladium/production/atoms/files/NHD%201999%20Draft%20Standards%20-%20Capture%20conditions.PDF.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessOmission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_CompletenessCommission>
      <mdq:result>
        <mdq:DQ_DescriptiveResult>
          <mdq:statement>
            <gco:CharacterString> The completeness of the data reflects the content of the sources, which most often are the published USGS topographic quadrangle and/or the USDA Forest Service Primary Base Series (PBS) map. The USGS topographic quadrangle is usually supplemented by Digital Orthophoto Quadrangles (DOQs). Features found on the ground may have been eliminated or generalized on the source map because of scale and legibility constraints. In general, streams longer than one mile (approximately 1.6 kilometers) were collected. Most streams that flow from a lake were collected regardless of their length. Only definite channels were collected so not all swamp/marsh features have stream/rivers delineated through them. Lake/ponds having an area greater than 6 acres were collected. Note, however, that these general rules were applied unevenly among maps during compilation. Reach codes are defined on all features of type stream/river, canal/ditch, artificial path, coastline, and connector. Waterbody reach codes are defined on all lake/pond and most reservoir features. Names were applied from the GNIS database. Detailed capture conditions are provided for every feature type in the Standards for National Hydrography Dataset available online through https://prd-wret.s3-us-west-2.amazonaws.com/assets/palladium/production/atoms/files/NHD%201999%20Draft%20Standards%20-%20Capture%20conditions.PDF.</gco:CharacterString>
          </mdq:statement>
        </mdq:DQ_DescriptiveResult>
      </mdq:result>
    </mdq:DQ_CompletenessCommission>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_AbsoluteExternalPositionalAccuracy>
      <mdq:evaluationMethod>
        <mdq:DQ_EvaluationMethod>
          <mdq:evaluationMethodDescription>
            <gco:CharacterString>Statements of horizontal positional accuracy are based on accuracy statements made for U.S. Geological Survey topographic quadrangle maps. These maps were compiled to meet National Map Accuracy Standards. For horizontal accuracy, this standard is met if at least 90 percent of points tested are within 0.02 inch (at map scale) of the true position. Additional offsets to positions may have been introduced where feature density is high to improve the legibility of map symbols. In addition, the digitizing of maps is estimated to contain a horizontal positional error of less than or equal to 0.003 inch standard error (at map scale) in the two component directions relative to the source maps. Visual comparison between the map graphic (including digital scans of the graphic) and plots or digital displays of points, lines, and areas, is used as control to assess the positional accuracy of digital data. Digital map elements along the adjoining edges of data sets are aligned if they are within a 0.02 inch tolerance (at map scale). Features with like dimensionality (for example, features that all are delineated with lines), with or without like characteristics, that are within the tolerance are aligned by moving the features equally to a common point. Features outside the tolerance are not moved; instead, a feature of type connector is added to join the features.</gco:CharacterString>
          </mdq:evaluationMethodDescription>
        </mdq:DQ_EvaluationMethod>
      </mdq:evaluationMethod>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:nameOfMeasure>
            <gco:CharacterString>Horizontal Positional Accuracy Report</gco:CharacterString>
          </mdq:nameOfMeasure>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_AbsoluteExternalPositionalAccuracy>
  </mdq:report>
  <mdq:report>
    <mdq:DQ_AbsoluteExternalPositionalAccuracy>
      <mdq:evaluationMethod>
        <mdq:DQ_EvaluationMethod>
          <mdq:evaluationMethodDescription>
            <gco:CharacterString>Statements of vertical positional accuracy for elevation of water surfaces are based on accuracy statements made for U.S. Geological Survey topographic quadrangle maps. These maps were compiled to meet National Map Accuracy Standards. For vertical accuracy, this standard is met if at least 90 percent of well-defined points tested are within one-half contour interval of the correct value. Elevations of water surface printed on the published map meet this standard; the contour intervals of the maps vary. These elevations were transcribed into the digital data; the accuracy of this transcription was checked by visual comparison between the data and the map.</gco:CharacterString>
          </mdq:evaluationMethodDescription>
        </mdq:DQ_EvaluationMethod>
      </mdq:evaluationMethod>
      <mdq:measure>
        <mdq:DQ_MeasureReference>
          <mdq:nameOfMeasure>
            <gco:CharacterString>Vertical Positional Accuracy Report</gco:CharacterString>
          </mdq:nameOfMeasure>
        </mdq:DQ_MeasureReference>
      </mdq:measure>
    </mdq:DQ_AbsoluteExternalPositionalAccuracy>
  </mdq:report>
</mdq:DQ_DataQuality>
```


https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/CSDGM-194_FY14_Metadata_DaikiMaru_2014-csdgm.xml

  ERROR: FGDC reader: Conversion of dateTime string to object failed


https://github.com/chris-macdermaid/gis-examples/blob/main/DataQuality/xml/Cadastre-csdgm.xml

  ERROR: FGDC reader: Conversion of dateTime string to object failed

