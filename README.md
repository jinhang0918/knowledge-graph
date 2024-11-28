
#数据源
美国能源信息署eia网站https://www.eia.gov/electricity/data/eia860/
#raw_data：从该网站下载下来的部分文件，包含全美两万多机组信息
#TX_data：通过dataprocess.ipynb这一个数据处理文件处理后，筛选出德克萨斯州的机组信息
##Generator_TX：德克萨斯所有机组信息（因为后续便于生成不同类型的节点，故把这一个文件又分为下面四种机组文件）
##Solar_TX：太阳能机组
##Wind_TX：风电机组
##Multifuel_TX：混合燃料机组
##Other_generator_TX：其他机组
###注：本项目主要关注这些文件中的Utility Name（公司信息）；Plant Code + Generator ID（机组名称）；County（机组所在的县）；Technology（机组的类型比如天然气，石油气等等）
#dataprocess.ipynb：数据处理文件，用于将下载下来的.xlsx文件转变为.csv文件、将TX机组筛选出来形成新文件
#main.ipynb：主程序
