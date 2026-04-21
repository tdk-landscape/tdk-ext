# =============================================================================
# 🎯 TDK-EXT - Extensions and IDE Components
# =============================================================================
# This is the Tiltfile entry point for the tdk-ext repo.
# It exports UI enhancements and IDE components.
#
# Usage:
#   v1alpha1.extension_repo(name='tdk-ext', url='https://github.com/tdk-landscape/tdk-ext')
#   load('ext://tdk-ext', 'load_ui_enhancements', ...)
# =============================================================================

# UI Enhancements
load('./ui-enhancements/tiltfile.py', _load_ui_enhancements='load_ui_enhancements')

# =============================================================================
# RE-EXPORTS
# =============================================================================

load_ui_enhancements = _load_ui_enhancements

# =============================================================================
# IDE COMPONENTS PATHS
# =============================================================================

def get_ide_components_path():
    """Return the path to IDE components."""
    return './ide-components'

def get_file_browser_script():
    """Return the path to file browser server script."""
    return './ide-components/file_browser/server.py'

def get_code_viewer_script():
    """Return the path to code viewer server script."""
    return './ide-components/code_viewer/server.py'

def get_config_inspector_script():
    """Return the path to config inspector server script."""
    return './ide-components/config_inspector/server.py'

def get_code_executor_script():
    """Return the path to code executor server script."""
    return './ide-components/code_executor/server.py'

# =============================================================================
# PORTS
# =============================================================================

IDE_PORTS = {
    'file_browser': 9765,
    'code_viewer': 9766,
    'config_inspector': 9767,
    'code_executor': 9768,
}

print("✅ TDK Extensions loaded: UI enhancements and IDE components")
