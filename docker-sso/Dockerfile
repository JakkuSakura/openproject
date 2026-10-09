# Community SSO unlock image for OpenProject 17.9.1.
#
# OpenProject gates all OmniAuth SSO strategies (including OpenID Connect)
# behind the Enterprise-only `sso_auth_providers` token. This fork removes that
# gate for the OpenID Connect strategy only, so a Community instance can log in
# against Keycloak using an env-seeded provider (OPENPROJECT_OPENID__CONNECT_*).
#
# Base image is pinned to the v17.9.1 digest of openproject/openproject:17.
FROM docker.io/openproject/openproject@sha256:1931b0bcdceb07c38293c3afafa7fe3da09e9fa76144604b92813d6c6d05c695

COPY modules/auth_plugins/lib/open_project/plugins/auth_plugin.rb \
     /app/modules/auth_plugins/lib/open_project/plugins/auth_plugin.rb
