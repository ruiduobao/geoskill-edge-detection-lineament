---
name: geoskill-edge-detection-lineament
description: 'Canny/Sobel边缘检测+概率Hough变换提取线性构造，输出边缘栅格与线段GeoJSON'
---

# 边缘检测与线性构造提取 | Edge Detection and Lineament Extraction

(Fill in 2-3 paragraphs of Chinese introduction here: functionality, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'scikit-image' 'geopandas' 'shapely'
```

## Usage / 使用方法

### Basic usage

```bash
python geoskill-edge-detection-lineament.py --bbox 116.0 39.0 117.0 40.0 [other options]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-edge-detection-lineament.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real-world usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Primary output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is done locally; user data is never uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
