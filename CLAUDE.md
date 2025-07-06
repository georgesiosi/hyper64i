# 64-Cell Hyper-Stack I-Ching Memory Scheduler

## Project Overview

This project implements a fusion of ancient Chinese philosophy (I-Ching) and computer science theory, specifically combining Ryan Williams' √t space-time simulation theorem with a 6-dimensional hypercube memory scheduler.

## Core Concept

The **64-Cell Hyper-Stack Memory Scheduler** maps Williams' √t space-time simulation theorem onto a 6-dimensional hypercube, where each of the 64 vertices corresponds to an I-Ching hexagram. This creates an intuitive debugging layer where memory cells have both computational and symbolic meaning.

## Technical Architecture

### Key Components
- **6-Bit Hypercube**: 64 nodes representing memory cells, connected by Hamming-1 transitions
- **Gray Code Traversal**: Ensures only one bit flips between adjacent cells, minimizing memory swap overhead
- **I-Ching Mapping**: Each hexagram corresponds to a binary state (yin=0, yang=1), providing semantic debugging context
- **Balanced Separators**: Leverages Williams' theorem for √t memory usage on planar execution graphs

### Performance Targets
- **1-D Stencil**: ≤ 0.6√t cells (~1900 states for t=10⁵) with ≤4× slowdown
- **Binary Tree**: ≤ 1024 states via subtree symmetry with ≤2× slowdown
- **Transformer**: 64 chunk states mapped to 64 cube cells with ≤1.5× slowdown

## File Structure

```
hyper64i/
├── CLAUDE.md                          # This file - project documentation
└── hypercube_iching_simulator.html    # Main application (self-contained)
```

## Features

### Interactive Visualization
- **Hypercube Display**: Circular 2D projection of 6D hypercube with 64 nodes
- **I-Ching Grid**: 8×8 grid showing all 64 hexagrams with visual line representations
- **Real-time Animation**: Gray code path visualization with smooth transitions
- **Click Navigation**: Direct jumping to any memory cell/hexagram

### Simulation Controls
- **Gray Code Walk**: Automated traversal following optimal memory access patterns
- **Random Jump**: Test arbitrary memory access patterns
- **Workload Types**: 
  - 1-D Stencil (Grid computation)
  - Binary Tree Evaluation
  - Transformer Neural Network layers
  - Custom DAG processing
- **Speed Control**: Adjustable animation timing (100ms - 2000ms)

### Monitoring & Analytics
- **Memory Statistics**: Real-time usage tracking and separator size calculation
- **Algorithm Trace**: Live log of memory operations and transitions
- **Path History**: Complete record of visited cells and traversal patterns
- **Performance Metrics**: √t complexity calculations and efficiency measurements

## Theoretical Significance

This work represents a novel intersection of:
- **Complexity Theory**: Williams' √t space-time simulation
- **Graph Algorithms**: Hypercube traversal and Gray code sequences  
- **Traditional Knowledge**: 6,000-year-old I-Ching hexagram system
- **Memory Management**: Optimal locality and debugging visualization

The key insight is that **adjacent hexagrams differ by exactly one line**, which maps perfectly to Hamming-1 transitions in the hypercube, ensuring optimal memory locality while providing meaningful symbolic context.

## Development Guidelines

### Code Organization
- Single HTML file architecture for maximum portability
- Vanilla JavaScript (no external dependencies)
- CSS Grid and Flexbox for responsive layout
- SVG for hypercube visualization
- ES6+ features for modern browser compatibility

### Adding New Features
When extending the simulator, consider:

1. **Memory Cell Operations**: New algorithms should respect Gray code constraints
2. **Visualization Updates**: Maintain consistency between hypercube and I-Ching views
3. **Performance Monitoring**: Include √t complexity calculations for new workloads
4. **I-Ching Integration**: Preserve symbolic meaning in hexagram transitions

### Future Extensions
- **Real DAG Processing**: Implement actual stencil/tree/transformer workloads
- **3D Hypercube Visualization**: More accurate geometric representation
- **Separator Highlighting**: Visual representation of graph separators
- **Performance Benchmarking**: Real-time comparison against baseline algorithms
- **Custom Workload Designer**: User-defined computation graphs
- **AI Integration**: Neural network inference optimization
- **Quantum Adaptation**: Extension to quantum computing memory management

## Usage Instructions

### Quick Start
1. Open `hypercube_iching_simulator.html` in a modern web browser
2. Click "Start Gray Code Walk" to begin automated simulation
3. Use control panel to adjust speed and workload types
4. Click any hexagram or hypercube node for direct navigation
5. Monitor real-time statistics and algorithm trace

### Advanced Features
- **Modal Documentation**: Click "About" in footer for detailed theoretical background
- **Workload Comparison**: Switch between different computation types to see performance differences
- **Path Analysis**: Use algorithm trace to understand memory access patterns
- **Manual Navigation**: Click specific cells to test custom traversal sequences

## Related Work

This visualization is inspired by the broader **Conscious Stack Design** methodology, which focuses on aligning digital tools and workflows with human behavior to reduce digital chaos.

**Learn more**: [consciousstackdesign.com](https://consciousstackdesign.com)

## Technical Notes

### Browser Compatibility
- Modern browsers with ES6+ support
- SVG and CSS Grid capability required
- Tested on Chrome, Firefox, Safari, Edge

### Performance Considerations
- 64-cell limit ensures smooth animation
- Gray code calculations are O(1) per transition
- Memory usage scales with visualization complexity
- Responsive design adapts to different screen sizes

### Accessibility
- Keyboard navigation support (Escape to close modals)
- High contrast color scheme for visibility
- Semantic HTML structure for screen readers
- Responsive design for mobile devices
