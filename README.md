# React-Predictor-Cam

A React component library to visualize predictions and Grad-CAM overlays for image classification models.

![Demo](path-to-demo-gif-or-screenshot)

---

## Features
- Easy model input and output integration.
- Grad-CAM overlay visualization.
- React component with customizable styles.


## Installation
```bash
npm install react-predictor-cam
```

## Usage
```tsx
import React from "react";
import { ModelViewer } from "react-predictor-cam";

const App = () => {
  return (
    <ModelViewer
      modelUrl="/path-to-model"
      inputShape={[224, 224]}
      outputLabels={["Cat", "Dog", "Horse"]}
      gradCamData={gradCamArray}
    />
  );
};

export default App;
```

## Props
| Prop          | Type          | Description                            | Required |
|---------------|---------------|----------------------------------------|----------|
| `modelUrl`    | `string`      | URL of the TensorFlow.js model.        | Yes      |
| `inputShape`  | `[number, number]` | Shape of the input image.           | Yes      |
| `outputLabels`| `string[]`    | Array of output labels.                | Yes      |
| `gradCamData` | `number[][]`  | Grad-CAM heatmap data.                 | No       |


## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
MIT

