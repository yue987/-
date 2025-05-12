

<头>
    <meta charset="UTF-8">
    <title>AI创意LOGO生成器</title>
    <样式>
        /* 响应式布局 */
        .设计面板 {
            显示：网格;
            网格列模板：300像素 1填充单位;
            间隙：20像素;
            
        输入：}
 
        /* 参数控制区 */
        .controls {
            背景: #f5f5f5;
            内边距：15px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
 
        /* 实时预览区 */
        #logo-preview {
            最小高度: 400px;
            display: flex;
            对齐项目：居中；
            项目对齐方式：居中；
            背景：白色；
            边框: 2px 虚线 #ddd;
        }
 
        /* 动态参数调节 */
        参数滑块
            display: flex;
            margin: 15px 0;
            对齐项目：居中；
        }
        参数滑块标签 {
            宽度：80px;
        }
    

<身体>
    
        
        
            LOGO参数设置
            
            
                <label>品牌名称：</label>
                <输入 type="text" id="brandName" placeholder="输入品牌名称">
            </div>
 
            
                <label>图标尺寸：</label>
                <输入 type="范围" id="图标大小" min="50" max="200" value="100">
            </div>
 
            
                <label>主色调：</label>
                <输入 type="颜色" id="主颜色" value="#3174f0">
            </div>
 
            <button onclick="generateLogo()">生成LOGO</button>
        </div>
 
        
        
            
                
            </svg>
        </div>
    </div>
 
    <脚本>
        // 动态生成LOGO的核心逻辑
        function generateLogo() {
            const brandName = document.getElementById('brandName').value;
            const iconSize = document.getElementById('iconSize').value;
            const mainColor = document.getElementById('mainColor').value;
 
            const svg = document.getElementById('logo-svg');
            svg.innerHTML  = `
                <rect x="10" y="10" width="80" height="80" fill="${mainColor}" rx="15"/>
                <text x="50%" y="50%"
                      text-anchor="middle"
                      dominant-baseline="middle"
                      font-size="${iconSize/3}px"
                      填充="白色">
                    ${品牌名称}
                </text>
            ```
```
        }
 
        // 初始化生成
        generateLogo();
    </script>
</主体>
</html>
