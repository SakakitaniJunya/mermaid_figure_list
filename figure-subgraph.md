````mermaid
%%{
  init: {
    'theme': 'base',
    'themeVariables': {
      'primaryColor': '#BB2528',
      'primaryTextColor': '#fff',
      'primaryBorderColor': '#7C0000',
      'lineColor': '#F8B229',
      'secondaryColor': '#006100',
      'tertiaryColor': '#2A303C'
    }
  }
}%%
graph TB

	subgraph Develop["Develop Study"]
		subgraph C#
			CodeWar
			DDD-Develop
		end
		subgraph JS
			subgraph NextJS
				DDD
				Test
			end
			JS-App-timer
		end
		subgraph AWS
			Udemy
			APP-Release
		end
	end

	subgraph Playing["Playing"]
		subgraph MermaidJS
			Create-Graph
			Color-Setting
		end
	end

    ```
````
