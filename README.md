Nope it does not work

1. [ERROR] ReferenceError: window is not defined
   ```ts
   canvas.toBlob(
      (blob) => {
        if (!blob) {
          return;
        }
        const objectURL = window.URL.createObjectURL(blob);
        setCanvasOverlay(objectURL);
      },
      'image/jpeg',
      0.75
    );
   ```