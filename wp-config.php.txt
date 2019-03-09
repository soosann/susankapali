<?php
/**
 * The base configuration for WordPress
 *
 * The wp-config.php creation script uses this file during the
 * installation. You don't have to use the web site, you can
 * copy this file to "wp-config.php" and fill in the values.
 *
 * This file contains the following configurations:
 *
 * * MySQL settings
 * * Secret keys
 * * Database table prefix
 * * ABSPATH
 *
 * @link https://codex.wordpress.org/Editing_wp-config.php
 *
 * @package WordPress
 */

// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define( 'DB_NAME', 'codeanddesign' );

/** MySQL database username */
define( 'DB_USER', 'root' );

/** MySQL database password */
define( 'DB_PASSWORD', '' );

/** MySQL hostname */
define( 'DB_HOST', 'localhost' );

/** Database Charset to use in creating database tables. */
define( 'DB_CHARSET', 'utf8mb4' );

/** The Database Collate type. Don't change this if in doubt. */
define( 'DB_COLLATE', '' );

/**#@+
 * Authentication Unique Keys and Salts.
 *
 * Change these to different unique phrases!
 * You can generate these using the {@link https://api.wordpress.org/secret-key/1.1/salt/ WordPress.org secret-key service}
 * You can change these at any point in time to invalidate all existing cookies. This will force all users to have to log in again.
 *
 * @since 2.6.0
 */
define( 'AUTH_KEY',         ']HZXAKM0QE~%Fldh%b7##3-1&B)I;6_h/5y#CmA?C@]lqIT:@C^^&h&Dl&u9ha?d' );
define( 'SECURE_AUTH_KEY',  'HWL-fofc<7baS1Ua~2RVeeF Tr}05qPpzvq@4OAp&Np*v[`jq(j n:$!1*9=WPz.' );
define( 'LOGGED_IN_KEY',    'oq:a~C:}}m}t_6^8brGT q}R^SUFf{U$58*mk<9 VJRcfk54<R/0^7h=LmgNty(L' );
define( 'NONCE_KEY',        '; d  x-_ZguyAGV1>35#=LeO-ozU~Mt3sngcM[>9U7),e{>Az]XWyA,!S,k[k!e$' );
define( 'AUTH_SALT',        '-eB(iWiW[%kV}fvH4C=bbg]t](9&x8~KMz57KUEEUScEg&o oEb,{pXR1T>D`gR0' );
define( 'SECURE_AUTH_SALT', '/*^!=| 9v-f`{B*D51~oLHv%G*5r$g: C{:x-QLTA-y{Q9eyR-=XG<sf-+5#>$$6' );
define( 'LOGGED_IN_SALT',   'g|dCF3I4154*Z&BUmwXSOd98_u,~-~S:XbvG>KQPT[?>J+7=i$34I5X=cc@c8lIj' );
define( 'NONCE_SALT',       '$c_g1 zga25J+l2EIvCYh~N|uFN;hju.KVZif;6)pv`gX)c97D^(1_,uB0Jr3kG/' );

/**#@-*/

/**
 * WordPress Database Table prefix.
 *
 * You can have multiple installations in one database if you give each
 * a unique prefix. Only numbers, letters, and underscores please!
 */
$table_prefix = 'wp_';

/**
 * For developers: WordPress debugging mode.
 *
 * Change this to true to enable the display of notices during development.
 * It is strongly recommended that plugin and theme developers use WP_DEBUG
 * in their development environments.
 *
 * For information on other constants that can be used for debugging,
 * visit the Codex.
 *
 * @link https://codex.wordpress.org/Debugging_in_WordPress
 */
define( 'WP_DEBUG', false );

/* That's all, stop editing! Happy publishing. */

/** Absolute path to the WordPress directory. */
if ( ! defined( 'ABSPATH' ) ) {
	define( 'ABSPATH', dirname( __FILE__ ) . '/' );
}

/** Sets up WordPress vars and included files. */
require_once( ABSPATH . 'wp-settings.php' );
