dataArray(self,coords, values=None,dtype=None):
        Create a dataArray  


**index( list of values ):**        Create a coord object from list of values

    pp.index(['Item 1', 'Item 2', 'Item 3'])
|**Function** (parameters)|Description|
|--|--|
|[`read_table`](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_table.html#pandas.read_table "pandas.read_table")(filepath_or_buffer[, sep, …])|Read general delimited file into DataFrame|

        


 createTime(self,date_start,date_end,freq='M',format='%Y.%m'):
        Create time index usign start and end dates and freq. The result is formated to format parameter
            Ex.
                cp.createTime('2016.01','2018.12')
                cp.createTime('2016.01','2016.12',freq='D',format='%d/%m/%Y')
        

		
  selfArray(self,index):
        Create an array from index
        
		
 changeIndex(self,array,oldIndex,newIndex,compareMode=1,defaultValue=None):
        Change index of a dataArray object.
            TODO: samples
        


    indexFromPandas(self,dataframe, columnName=None, removeEmpty=True):
         Return a pp.index from an column of a pandas dataframe.
        dataframe: pandas dataframe
        columnName: dataframe column name used for create cp.index. By default is created using the first column
        removeEmpty: True for remove empty rows
            Ex.
                cp.indexFromPandas(df)
                cp.indexFromPandas(df,"column10")
                        

		
    excelConnection(self,filepath, useOpenpyxl=False, dataOnly=True, readOnly=True ):
         Create excel object from filepath.
        filepath: path to excel file
        useOpenpyxl: True for use custom 
        dataOnly: True for view only the values, not formula
        readOnly: True for read only, False for write options
        Ex.
                cp.excel("\path\to\the\excelfile.xlsx")
        

    pandasFromExcel(self,excel,sheetName=None,namedRange=None,cellRange=None, indexes=None, driver='Driver={Microsoft Excel Driver (*.xls, *.xlsx, *.xlsm, *.xlsb)};DBQ=%s;READONLY=TRUE'):
         return a pandas dataframe from excel.
        excel: path to excel file or cp.excel object
        sheetName: sheet name to be read
        namedRange: name of the range to be read
        cellRange: used with sheetname, for read from a simple range
        indexes: Listo of columns names for convert to index of dataframe
            Ex.
                cp.pandasFromExcel(excelNode,"Sheet 1")
                cp.pandasFromExcel(excelNode,namedRange="name_range")
                cp.pandasFromExcel(excelNode,"Sheet 1",cellRange="A1:H10")

        


    indexFromExcel(self,excel, sheetName=None,namedRange=None,cellRange=None, columnName=None, removeEmpty=True):
         Return a cp.index from an excel file.
        excel: cp.excel object
        sheetName: sheet name to be read
        namedRange: name of the range to be read
        cellRange: used with sheetname, for read from a simple range
        columnName: dataframe column name used for create cp.index. By default is created using the first column
        removeEmpty: True for remove empty rows
            Ex.
                cp.indexFromExcel(excelNode,"Sheet 1")
                cp.indexFromExcel(excelNode,namedRange="name_range")
                cp.indexFromExcel(excelNode,namedRange="name_range", columnName="indicadores")
                        


    dataArrayFromExcel(self,excel, sheetName=None,namedRange=None,cellRange=None, indexes=None, valueColumns=None, indexColumnHeaders=None, replaceByIndex=None):
         Return a cp.cube from excel file.
            excel: cp.excel object
        sheetName: sheet name to be read
        namedRange: name of the range to be read
        cellRange: used with sheetname, for read from a simple range
        indexes: objects pp.index for perform change index
        valueColumns: string with column name of the dataframe where contain the values
                        pp.index with columns names for convert colums to index
        indexColumnHeaders: (optional) column names in pandas to parse with indexes. Used if header on dataframe is not equal to index identifiers.
        replaceByIndex: (optional) replace index used in valueColumns for this index. (using changeindex)

            Ex.
                cp.cubeFromExcel(excelNode,"Sheet 1",indexes=[indicadores],valueColumns="descuentos")
                cp.cubeFromExcel(excelNode,namedRange="nombre_rango",indexes=[indicadores],valueColumns=time)
        


    concatIndex(self, *args):
        
        Concatenates two or more indexes and/or atomic values into a single new index
        Return: new index
            Ex.
                cp.concatIndex(index1,index2,index3,value1,value2)
        


    yearsToTime(self,dataArray,yearsIndex,timeIndex,div=12):
         Convert dataArray indexed by anual index to a monthly index
        dataArray are the dataArray with annual values to be converted
        yearIndex: is the year index of the original matrix
        timeIndex: is the monthly index of the result
        div: is an optional parameter used as divisor of the annual values (the tipical value is 12)
        


    find(self,param1, param2, compareType=1, caseSensitive = True):
        
        param1: value or indexarray for compare
        param2: index compare to
        compareType: cp.exact=1, cp.start_with=2, cp.end_with=3, cp.contain=4  
        caseSensitive: able to differentiate between uppercase and lowercase (by default True)

        If param1 is a scalar (numeric or str) and param2 is an index:  return a dataArray indexed by param2 with True on ocurrences of param2
            Ex. result = pp.find("te", region, cp.end_with)
        If param1 is an index and param2 is an index too:  return a dataArray indexed by param1 and param2 with True on ocurrences of param1 on param2
            Ex. result = pp.find(subregion, region, cp.contain)

        


    choice(self,index,selection,includeAll=False):
        Return the element in the "selection" position of the index. 
        


    copyAsValues(self, source, targetId):
        Copy values of datArray "source" into dataArray with id 'targetId'. This function alter the definition of dataArray with 'targetId' identifier.
            source: dataArray/index from copy values
            targetId: identifier (string) of the target node 
        

    goalSeek(self,nodeIdX, nodeIdObjective, goal=0, startValue=1): 
         Finds the value of nodeIdX that makes nodeIdObjective equal to goal.
        nodeIdX: String with id of node X
        nodeIdObjective: String with id of node X
        


    plot(self,fig, **kwargs):
        
        Generate HTML with plotly chart
        Params:
            fig: Pandas Dataframe , DataArray, or plotly fig
            x: column for the x axis
            y: column for the y axis
            series: column or list of columns for de series,

            other params:  layout,kind='scatter', title='', xTitle='', yTitle='', zTitle='', theme=None, colors=None, colorscale=None, fill=False, width=None, mode='lines', symbol='dot', size=12, barmode='', sortbars=False, bargap=None, bargroupgap=None, bins=None, histnorm='', histfunc='count', orientation='v', boxpoints=False, annotations=None, keys=False, bestfit=False, bestfit_colors=None, categories='', x='', y='', z='', text='', gridcolor=None, zerolinecolor=None, margin=None, subplots=False, shape=None, asFrame=False, asDates=False, asFigure=False, asImage=False, dimensions=(1116, 587), asPlot=False, asUrl=False, online=None, **kwargs
            reference: https://plot.ly/ipython-notebooks/cufflinks/#cufflinks-reference
        


    ejemplo_aggregatre(self,aa):
		 TODO/ comment
		


    aggregate(self,dataArray,mapInfo,sourceIndex,targetIndex):
         Aggregates the values in DataArray to generate the result indexed by  targetIndex.
            Map gives the value of targetIndex for each element of sourceIndex

            Example for aggregating time information into annual index the syntax is:
                cp.aggregate(dataArray, map, time, years )
        


    nestedGroupby(self,dataArray, groupby, applyFn):
         Apply "applyFn" to all dims in "groupby" of the "dataArray"
        


    apply(self, obj, applyFn):
         Apply "applyFn" to "obj" where obj can be DataArray or Index
        



    cascadeVolume(self,demand,ranges,consumption_range_index=None):
        TODO Comment
        Ex:
                pp.cascadeVolume(cantidades,limites_rango_consum)
                pp.cascadeVolume(cantidades,limites_rango_consum,"rangos_consumo")
                pp.cascadeVolume(cantidades,limites_rango_consum,rangos_consumo)
        



    bandAllocation(self,demand,ranges,consumption_range_index=None):
        TODO Comment
            Ex:
                cp.bandAllocation(cantidades,limites_rango_consum)
                cp.bandAllocation(cantidades,limites_rango_consum,"rangos_consumo")
                cp.bandAllocation(cantidades,limites_rango_consum,rangos_consumo)
        




    dispatch(self,contract_vol, contract_price, contract_index, demand):
        TODO comment
            Ex:
                cp.dispatch(contract_volumes,prices,contracts,demand)
        


    irr(self,flow, time_index ):
        Returns the Internal Rate of Return (IRR) of a series of periodic payments (negative values) and inflows (positive values). The IRR is the discount rate at which the Net Present Value (NPV) of the flows equals zero. 
            The variable flow must be indexed by time_index.

        If the cash flow never changes sign, cp.irr() has no solution and returns NAN (Not A Number).
        



    npv(self,rate, flow, time_index, offset = 1): 
        "Returns the Net Present Value (NPV) of a cash flow with equally spaced periods. The flow parameter must contain a series of periodic payments (negative values) and inflows (positive values), indexed by time_index.
            The optional offset parameter especifies the offset of the first value relative to the current time period. By default, offset is set to 1, indicating that the first value is discounted as if it is one step in the future
        



    lookup(self,dataArray, dataMap, sharedIndex): 
        
        Returns the value of dataArray indexed by the index of dataMap.
        dataArray must be indexed by sharedIndex and dataArray values must correspond to elements of sharedIndex.
        For example: Let's say you have a cube with an estimated inflation rate by Country ("inflation_rate" is the name of the cube; "country" is the name of the index) and you want to assign it to the corresponding Company depending on its location. On the other hand, there's a many-to-one map where each Company is allocated to a single Country ("country_to_company_allocation"). The sharedIndex, in this case, is Country ("country").
        As a result, 
            pp.lookup( inflation_rate , country_to_company_allocation , country )
        will return the estimated inflation rate by Company.
        
        


    copyIndex(self,dataArray):
        Generate a pp.index with current unique values of the dataArray. 
        The dataArray must have only one dimension
        


    dynamic(self,dataArray,index,shift, initialValues=None):
        
        Perform cyclic calculations betwwen nodes.
        cube: cp.cube to evaluate
        index: Index to shift 
        shift: amount of elemnts to shift. Can be positive or negative
        initialValues: (optional), initial values to apply to first "shift" elemnts


> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU3NzY1MDE2MSwtMzYyNDA4NDQxXX0=
-->